# Manus × IBGE — Auditoria Pública de uma IA Agente
<img width="1600" height="450" alt="ChatGPT Image 18 de jul  de 2026, 12_14_49" src="https://github.com/user-attachments/assets/5fa9cba7-903e-469f-af63-e47cb5dacc33" />

Auditoria independente de duas entregas produzidas pela Manus para indicadores municipais do IBGE.
> Dado correto não é sinônimo de entrega confiável. Sem cobertura,
> rastreabilidade, documentação e validação, até milhares de valores certos
> podem sustentar uma conclusão errada.

**Responsável técnico:** Igor Vasconcellos  
**Versão pública:** V1.0

## Ecossistema público do projeto

Este trabalho integra diferentes plataformas públicas, cada uma com uma função específica no processo de publicação, documentação e análise dos dados.

* **Dashboard no Tableau Public:** [Acessar visualização](https://public.tableau.com/views/Manus-AuditoriapblicadeIAv1_0/Capa?:language=pt-BR&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)
* **Dataset no Kaggle:** [Acessar conjunto de dados](https://www.kaggle.com/datasets/israelthesheep/manus-ibge-auditoria-pblica-de-ia)
* **Notebook no Kaggle:** [Acessar análise reproduzível](https://www.kaggle.com/code/israelthesheep/01-vis-o-geral-da-auditoria-manus-ibge)
* **Repositório no GitHub:** [Acessar projeto](https://github.com/israelthesheep/manus-ibge-auditoria)
* **Artigo no Medium:** [Acessar artigo](https://medium.com/@igor.vasconcellos/dado-correto-n%C3%A3o-basta-uma-auditoria-p%C3%BAblica-de-uma-ia-agente-com-dados-do-ibge-49501fc4aeed)

## Resultado principal

| Métrica | Rodada 01 | Rodada 02 |
|---|---:|---:|
| Pontuação | 57,13 | 86,38 |
| Classificação global | Insuficiente para uso analítico | Utilizável com ressalvas |
| Cobertura de indicadores | 25% | 75% |
| Cobertura funcional-temporal | 31,25% | 68,75% |
| Condições bloqueadoras | 4 | 1 |

Na Rodada 02 foram auditados **61.273 registros**, correspondentes a **5.571 municípios**, sem divergências reais nos valores efetivamente materializados.

A área territorial permaneceu ausente. A conclusão consolidada é:

`MELHORIA_SUBSTANCIAL_COM_INCOMPLETUDE_REMANESCENTE`

## Escopo deste repositório

Este repositório contém exclusivamente derivados públicos sanitizados:

- sete arquivos CSV validados;
- metodologia pública;
- dicionário resumido e inventário completo dos campos;
- notas de cobertura e limitações;
- linhagem pública;
- roteiro de verificação e reprodução pública;
- documentação do Tableau;
- manifestos, checklist e registros de governança.

Não são publicados:

- o dossiê técnico congelado;
- evidências brutas da Manus;
- arquivos originais `Untitled`;
- credenciais, tokens ou chaves;
- arquivos `.env` ou `kaggle.json`;
- caches, logs internos ou caminhos locais sensíveis.

## Estrutura

```text
.
├── data/          CSVs públicos validados
├── docs/          metodologia, dicionários, limitações e reprodução
├── notebooks/     orientação sobre notebooks públicos
├── tableau/       painel público e Notas Técnicas
└── governance/    sanitização, integridade e decisão da etapa
```

## Arquivos de dados

| Arquivo | Conteúdo |
|---|---|
| `manus_ibge_pontuacao_dimensoes_rodadas_01_02_v01.csv` | Pontuação comparativa por critério |
| `manus_ibge_indicadores_comparativos_rodadas_01_02_v01.csv` | Indicadores sintéticos das duas rodadas |
| `manus_ibge_cobertura_indicadores_periodos_v01.csv` | Cobertura de indicadores e períodos |
| `manus_ibge_achados_auditoria_v01.csv` | Achados consolidados da auditoria |
| `manus_ibge_classificacoes_limitacoes_v01.csv` | Classificações e limitações |
| `manus_ibge_dados_entregues_rodada_02_v01.csv` | 61.273 registros auditados da Rodada 02 |
| `manus_ibge_dim_municipios_rodada_02_v01.csv` | Dimensão pública com 5.571 municípios |

Todos os CSVs utilizam codificação UTF-8 e separador `;`.

## Visualização pública

[Tableau Public — Manus: Auditoria pública de IA](https://public.tableau.com/app/profile/israel.sheep/viz/Manus-AuditoriapblicadeIAv1_0/Capa?publish=yes)

As Notas Técnicas de cada painel estão relacionadas em [`tableau/README.md`](tableau/README.md).

## Integridade e reprodução

Os hashes SHA-256 são registrados em `governance/manifesto_publicacao_publica.txt`.

O roteiro de verificação está em [`docs/roteiro_reproducao.md`](docs/roteiro_reproducao.md).

## Fonte e atribuição

Os indicadores municipais têm como fonte de referência o Instituto Brasileiro de Geografia e Estatística — IBGE.

A auditoria, as transformações públicas, as classificações e a organização editorial são de responsabilidade de Igor Vasconcellos.

Este projeto é independente e não representa endosso institucional do IBGE ou da Manus.

## Licenciamento

- dados derivados e documentação: **CC BY 4.0**;
- scripts e códigos: **MIT**;
- conteúdos e direitos de terceiros não são relicenciados.

Consulte [`LICENSE`](LICENSE), [`LICENSE-CODE`](LICENSE-CODE) e [`LICENSE-DATA-DOCS`](LICENSE-DATA-DOCS).
