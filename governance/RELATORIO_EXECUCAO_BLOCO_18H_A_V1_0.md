# Relatório de Execução — Bloco 18H-A — V1.0

## Identificação

| Campo | Valor |
|---|---|
| Projeto | Manus × IBGE — Auditoria Pública de uma IA Agente |
| Bloco | 18H-A — Preparação do Pacote GitHub Sanitizado |
| Data | 2026-07-18 |
| Responsável técnico | Igor Vasconcellos |
| Pacote | `20_camada_publica/02_github_sanitizado` |
| Publicação realizada | Não |
| Push realizado | Não |

## Objetivo

Preparar um pacote local, técnico-editorial e sanitizado para futura publicação no GitHub, sem alterar o dossiê técnico congelado e sem realizar publicação, commit ou push.

## Estado de entrada

A execução partiu dos seguintes estados aprovados:

- camada técnica encerrada e congelada;
- dossiê técnico V1.0;
- derivados públicos gerados;
- QA dos derivados aprovado;
- Google Drive validado;
- upload manual validado;
- Tableau V1.0 concluído e publicado.

## Dossiê técnico de referência

```text
DOSSIÊ_TECNICO=DOSSIÊ_TECNICO_V1_0
ARQUIVOS_CONGELADOS=456
BYTES_CONGELADOS=79265230
SHA256_RAIZ=326ef01d169ebba93e6f100a354ef3fb554502e720cc98173118a3bfeb521e39
```

O dossiê técnico permaneceu intocado e não foi copiado para o pacote GitHub.

## Diagnóstico inicial

Foi confirmado que:

- a raiz geral do projeto não era um repositório Git;
- a área `02_github_sanitizado` continha somente um README provisório;
- as centrais privadas estavam presentes e separadas;
- os sete CSVs públicos esperados estavam disponíveis;
- os documentos públicos do Tableau estavam disponíveis;
- os originais da Manus e os arquivos `Untitled` permaneceram fora do escopo GitHub.

## Fonte canônica

Os CSVs foram copiados de:

```text
20_camada_publica/03_tableau/dados_derivados
```

As cópias foram comparadas com:

- a publicação operacional do Tableau;
- o pacote normalizado do projeto;
- os hashes anteriormente validados.

## Dados incluídos

| Controle | Resultado |
|---|---:|
| Arquivos CSV | 7 |
| Registros granulares da Rodada 02 | 61.273 |
| Municípios | 5.571 |
| Registros de achados | 7 |
| Registros de classificações | 6 |
| Registros de cobertura | 6 |
| Registros comparativos | 6 |
| Critérios de pontuação | 9 |
| Divergências reais | 0 |

Todos os CSVs foram reconhecidos como UTF-8, com separador `;` e cabeçalhos válidos.

## Documentação criada ou consolidada

Foram preparados:

- README principal;
- metodologia pública atualizada;
- notas de cobertura e limitações;
- dicionário resumido;
- inventário completo de campos;
- linhagem pública sanitizada;
- roteiro de reprodução pública;
- documentação do Tableau;
- orientação pública para notebooks;
- política de sanitização;
- licenças públicas;
- checklist de sanitização.

## Tableau

Foi registrado o link público:

<https://public.tableau.com/app/profile/israel.sheep/viz/Manus-AuditoriapblicadeIAv1_0/Capa?publish=yes>

Também foram registrados os links das quatro Notas Técnicas públicas.

Não foram inventados links para Google Drive, Kaggle ou Medium, pois URLs públicas desses destinos não estavam registradas nos artefatos consultados.

## Licenciamento

Foi adotado licenciamento duplo:

- MIT para scripts e códigos;
- CC BY 4.0 para dados derivados e documentação.

O pacote registra:

- o IBGE como fonte de referência dos indicadores;
- Igor Vasconcellos como responsável técnico pela auditoria e pelas transformações;
- a preservação dos direitos de terceiros;
- a ausência de endosso institucional do IBGE ou da Manus.

## Controles de segurança

| Controle | Resultado |
|---|---:|
| Nomes de arquivos proibidos | 0 |
| Padrões sensíveis em conteúdo | 0 |
| Credenciais | 0 |
| Tokens | 0 |
| Chaves privadas | 0 |
| Caminhos absolutos locais | 0 |
| Arquivos `Untitled` | 0 |
| Arquivos `.env` | 0 |
| Arquivos `kaggle.json` | 0 |
| ZIPs | 0 |
| Logs internos | 0 |
| Caches | 0 |

## Validação estrutural

| Controle | Resultado |
|---|---:|
| Falhas nas cópias dos CSVs | 0 |
| Falhas nas quantidades de registros | 0 |
| Links locais verificados | 6 |
| Falhas em links locais | 0 |

## Manifesto público

O manifesto SHA-256 cobre o núcleo publicável de 20 arquivos.

```text
ARQUIVOS_NO_MANIFESTO=20
ARQUIVOS_APROVADOS=20
ARQUIVOS_REPROVADOS=0
RC_VALIDACAO=0
SHA256_MANIFESTO=73509ab035167ea8f7eeaa3e281ae1fcdb38eb71ff710df421781116713f0002
```

Os registros finais de governança não integram o próprio manifesto, evitando autorreferência circular.

## Checkpoint do pacote

Após a criação do manifesto e do checklist:

```text
ARQUIVOS_ATUAIS=22
BYTES_ATUAIS=12139572
```

O relatório e a decisão formal são acrescentados após esse checkpoint.

## Restrições preservadas

Não foram realizados:

- alteração do dossiê técnico;
- acesso ao conteúdo das centrais privadas;
- inclusão de evidências brutas;
- inclusão dos originais da Manus;
- inicialização de repositório Git;
- configuração de remoto;
- commit;
- push;
- publicação no GitHub.

## Resultado da execução

```text
BLOCO_18H_A_EXECUTADO=SIM
PACOTE_LOCAL_SANITIZADO=SIM
VALIDACAO_ESTRUTURAL=APROVADA
VALIDACAO_SEGURANCA=APROVADA
VALIDACAO_MANIFESTO=APROVADA
PUBLICACAO_REALIZADA=NAO
PUSH_REALIZADO=NAO
```

## Conclusão

O pacote local GitHub sanitizado V1.0 foi preparado com dados públicos validados, documentação atualizada, licenciamento explícito, rastreabilidade pública e controles de segurança.

O pacote está tecnicamente apto para a decisão formal do Bloco 18H-A, permanecendo a publicação condicionada à confirmação expressa do responsável.

## Recuperação R1 — Formatação Markdown

A primeira validação final identificou duas falhas documentais de formatação:

- uma cerca Markdown não encerrada em `governance/checklist_sanitizacao.md`;
- uma cerca Markdown não encerrada em `tableau/README.md`.

A falha foi causada durante a transferência manual dos conteúdos pelo chat e não afetou:

- os sete CSVs;
- as quantidades de registros;
- os hashes dos dados;
- a segurança do pacote;
- as licenças;
- a separação das áreas privadas.

Resultado inicial:

```text
FALHAS_DOCUMENTAIS=2
RC_MANIFESTO_INICIAL=0
RC_SEGURANCA_INICIAL=1
SHA256_MANIFESTO_SUPERADO=760348af4092194255fa7edb11ba6c01da8394b2650fc546e296f0b7d0f4fc4d
```

Foram adicionadas as duas cercas de fechamento ausentes.

Resultado da recuperação:

```text
BLOCO_RECUPERACAO=BLOCO_18H_A_R1
FALHAS_MARKDOWN_R1=0
ARQUIVOS_NO_MANIFESTO_R1=20
ARQUIVOS_APROVADOS_R1=20
ARQUIVOS_REPROVADOS_R1=0
RC_MANIFESTO_R1=0
SHA256_MANIFESTO_R1=73509ab035167ea8f7eeaa3e281ae1fcdb38eb71ff710df421781116713f0002
```

O manifesto inicial foi formalmente substituído pelo manifesto R1.

A recuperação foi concluída sem alteração dos dados públicos e sem qualquer publicação ou push.