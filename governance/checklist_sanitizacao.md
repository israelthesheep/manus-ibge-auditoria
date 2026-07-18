# Checklist de Sanitização — GitHub V1.0

## Identificação

| Campo | Valor |
|---|---|
| Projeto | Manus × IBGE — Auditoria Pública de uma IA Agente |
| Bloco | 18H-A |
| Pacote | GitHub sanitizado V1.0 |
| Data da validação | 2026-07-18 |
| Responsável técnico | Igor Vasconcellos |
| Publicação realizada | Não |
| Push realizado | Não |

## Separação entre áreas

- [x] O pacote foi preparado exclusivamente em `20_camada_publica/02_github_sanitizado`.
- [x] A central privada permaneceu fora do pacote.
- [x] O cofre privado permaneceu fora do pacote.
- [x] O dossiê técnico congelado não foi alterado.
- [x] O dossiê técnico congelado não foi copiado.
- [x] Evidências brutas da Manus não foram incluídas.
- [x] Arquivos originais `Untitled` não foram incluídos.

## Dados públicos

- [x] Os sete CSVs públicos esperados foram localizados.
- [x] Os sete CSVs foram copiados da origem canônica.
- [x] As cópias foram comparadas com `cmp`.
- [x] As cópias apresentaram zero falhas.
- [x] Os hashes coincidem com a publicação operacional do Tableau.
- [x] Os hashes coincidem com o pacote normalizado do projeto.
- [x] Os arquivos utilizam codificação UTF-8.
- [x] Os arquivos utilizam separador `;`.
- [x] Os cabeçalhos foram reconhecidos.
- [x] As quantidades de registros foram validadas.

## Quantidades validadas

| Controle | Resultado |
|---|---:|
| Arquivos CSV | 7 |
| Registros granulares da Rodada 02 | 61.273 |
| Municípios | 5.571 |
| Divergências reais | 0 |
| Falhas de estrutura nos CSVs | 0 |

## Documentação

- [x] README principal criado.
- [x] Metodologia pública atualizada.
- [x] Notas de cobertura e limitações atualizadas.
- [x] Dicionário resumido incluído.
- [x] Inventário completo de campos incluído.
- [x] Linhagem pública sanitizada criada.
- [x] Roteiro de reprodução pública criado.
- [x] Documentação do Tableau criada.
- [x] Orientação pública para notebooks criada.
- [x] Política de sanitização incluída.
- [x] Links locais verificados.
- [x] Falhas em links locais: 0.

## Segurança

- [x] Arquivos `.env` ausentes.
- [x] Arquivo `kaggle.json` ausente.
- [x] Tokens ausentes.
- [x] Credenciais ausentes.
- [x] Chaves privadas ausentes.
- [x] Caminhos absolutos locais ausentes.
- [x] Nomes de estação ou VDI ausentes.
- [x] Usuários internos ausentes.
- [x] E-mails institucionais não autorizados ausentes.
- [x] Arquivos temporários ausentes.
- [x] Arquivos de cache ausentes.
- [x] ZIPs ausentes.
- [x] Logs internos ausentes.
- [x] Ocorrências nominais proibidas: 0.
- [x] Ocorrências de padrões sensíveis: 0.

## Licenciamento

- [x] Licenciamento duplo definido.
- [x] Scripts e códigos cobertos pela licença MIT.
- [x] Dados derivados e documentação cobertos pela CC BY 4.0.
- [x] Direitos de terceiros explicitamente preservados.
- [x] Fonte IBGE registrada.
- [x] Responsável pelas transformações identificado.
- [x] Ausência de endosso institucional explicitada.

## Integridade

- [x] Manifesto SHA-256 gerado.
- [x] Arquivos relacionados no manifesto: 20.
- [x] Arquivos aprovados na validação do manifesto: 20.
- [x] Arquivos reprovados na validação do manifesto: 0.
- [x] Código de retorno da validação: 0.

## Publicação

- [x] Pacote local preparado.
- [x] Repositório Git ainda não inicializado nesta pasta.
- [x] Nenhum remoto configurado nesta etapa.
- [x] Nenhum commit realizado nesta etapa.
- [x] Nenhum push realizado nesta etapa.
- [x] Publicação depende de confirmação expressa do responsável.

## Resultado

```text
CHECKLIST_SANITIZACAO_APROVADO
PACOTE_LOCAL_PREPARADO=SIM
PUBLICACAO_REALIZADA=NAO
PUSH_REALIZADO=NAO
```