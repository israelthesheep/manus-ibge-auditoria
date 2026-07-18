# Roteiro de reprodução pública

## Escopo

A reprodução pública permite:

- verificar a integridade dos arquivos;
- conferir estrutura, codificação e quantidade de registros;
- reproduzir comparações a partir dos CSVs publicados;
- conectar os dados a uma ferramenta analítica.

Ela não permite regenerar o experimento desde as evidências brutas, pois o dossiê técnico congelado e os arquivos originais da Manus não são distribuídos.

## Requisitos

Para as verificações descritas neste roteiro:

- terminal Bash, Git Bash ou equivalente;
- `sha256sum`;
- Python 3;
- nenhuma biblioteca Python externa.

## 1. Verificar os hashes

Na raiz do repositório, execute:

```bash
sha256sum -c governance/manifesto_publicacao_publica.txt
```

Todos os arquivos relacionados no manifesto devem retornar `OK`.

## 2. Conferir os CSVs

Os arquivos utilizam:

- codificação UTF-8;
- separador `;`;
- cabeçalho na primeira linha.

Execute:

```python
from csv import DictReader
from pathlib import Path

for arquivo in sorted(Path("data").glob("*.csv")):
    with arquivo.open(encoding="utf-8-sig", newline="") as entrada:
        leitor = DictReader(entrada, delimiter=";")
        registros = sum(1 for _ in leitor)
        print(f"{arquivo.name}: {registros} registros")
```

## 3. Totais esperados

| Arquivo | Registros |
|---|---:|
| `manus_ibge_achados_auditoria_v01.csv` | 7 |
| `manus_ibge_classificacoes_limitacoes_v01.csv` | 6 |
| `manus_ibge_cobertura_indicadores_periodos_v01.csv` | 6 |
| `manus_ibge_dados_entregues_rodada_02_v01.csv` | 61.273 |
| `manus_ibge_dim_municipios_rodada_02_v01.csv` | 5.571 |
| `manus_ibge_indicadores_comparativos_rodadas_01_02_v01.csv` | 6 |
| `manus_ibge_pontuacao_dimensoes_rodadas_01_02_v01.csv` | 9 |

## 4. Conferir o modelo de dados

Consulte:

- `docs/dicionario_dados.csv` para as definições públicas consolidadas;
- `docs/inventario_campos.csv` para a relação completa de campos, tipos inferidos, ordem, quantidade de não nulos e amostras;
- `docs/linhagem_publica.csv` para a relação entre os derivados públicos e as referências técnicas de origem.

## 5. Reproduzir as comparações

Os arquivos abaixo concentram os resultados comparativos:

- `manus_ibge_pontuacao_dimensoes_rodadas_01_02_v01.csv`;
- `manus_ibge_indicadores_comparativos_rodadas_01_02_v01.csv`;
- `manus_ibge_cobertura_indicadores_periodos_v01.csv`;
- `manus_ibge_achados_auditoria_v01.csv`;
- `manus_ibge_classificacoes_limitacoes_v01.csv`.

Eles permitem reproduzir:

- a evolução da pontuação;
- as diferenças entre as rodadas;
- as métricas de cobertura;
- as condições bloqueadoras;
- os achados e as classificações finais.

## 6. Reutilizar os dados granulares

Os dados granulares da Rodada 02 estão em:

```text
data/manus_ibge_dados_entregues_rodada_02_v01.csv
```

A dimensão municipal está em:

```text
data/manus_ibge_dim_municipios_rodada_02_v01.csv
```

Os dois arquivos podem ser relacionados pelo campo `codigo_municipio`.

## 7. Utilizar em ferramentas analíticas

Os CSVs podem ser conectados no:

- Tableau;
- Power BI;
- Python;
- R;
- ferramentas compatíveis com arquivos delimitados.

A visualização oficial está documentada em `tableau/README.md`.

## 8. Respeitar o limite interpretativo

Qualquer reprodução deve preservar as seguintes ressalvas:

- os valores são confiáveis somente na extensão auditada;
- a área territorial permaneceu ausente;
- a cobertura global permaneceu incompleta;
- a comparação está restrita às duas execuções avaliadas;
- os resultados não constituem prova causal generalizável.

## Resultado esperado

A reprodução pública deve confirmar:

```text
REGISTROS_AUDITADOS=61273
MUNICIPIOS=5571
DIVERGENCIAS_REAIS=0
COBERTURA_INDICADORES=75%
COBERTURA_FUNCIONAL_TEMPORAL=68.75%
CLASSIFICACAO_GLOBAL=UTILIZAVEL_COM_RESSALVAS
```