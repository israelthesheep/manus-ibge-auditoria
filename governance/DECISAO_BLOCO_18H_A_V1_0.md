# Decisão Formal — Bloco 18H-A — V1.0

## Identificação

| Campo | Valor |
|---|---|
| Projeto | Manus × IBGE — Auditoria Pública de uma IA Agente |
| Bloco | 18H-A — Preparação do Pacote GitHub Sanitizado |
| Data | 2026-07-18 |
| Responsável técnico | Igor Vasconcellos |
| Objeto | Aprovação do pacote local sanitizado para futura publicação no GitHub |

## Objeto da decisão

Avaliar se o pacote preparado em `20_camada_publica/02_github_sanitizado` atende aos requisitos técnicos, editoriais, documentais, de integridade e de segurança definidos para a futura publicação pública no GitHub.

Esta decisão não autoriza publicação automática, criação de repositório remoto ou execução de push.

## Bases consideradas

Foram considerados:

- o encerramento e congelamento da camada técnica;
- o dossiê técnico V1.0;
- os derivados públicos aprovados;
- o QA dos derivados públicos;
- a publicação operacional no Google Drive;
- a validação do upload manual;
- o pacote normalizado do projeto;
- o encerramento da etapa Tableau V1.0;
- o checklist de sanitização;
- o relatório de execução do Bloco 18H-A;
- o manifesto SHA-256 do núcleo publicável.

## Integridade dos dados

Os sete CSVs incluídos no pacote:

- foram copiados da origem canônica;
- permaneceram idênticos às fontes validadas;
- apresentaram hashes equivalentes nas cópias operacionais;
- tiveram estrutura e quantidades de registros verificadas;
- não apresentaram falhas de cópia ou leitura.

## Segurança

A validação não localizou:

- credenciais;
- tokens;
- chaves privadas;
- caminhos absolutos locais;
- nomes de estação ou VDI;
- usuários internos;
- arquivos `.env`;
- arquivos `kaggle.json`;
- arquivos originais `Untitled`;
- ZIPs;
- caches;
- logs internos;
- nomes de arquivos proibidos.

## Escopo público aprovado

O pacote contém somente:

- dados derivados sanitizados;
- documentação pública;
- metodologia;
- dicionários e inventários de campos;
- notas de cobertura e limitações;
- linhagem pública;
- roteiro de reprodução;
- documentação do Tableau;
- licenças;
- controles públicos de governança.

## Conteúdo excluído

Permanecem fora do pacote:

- o dossiê técnico congelado;
- as evidências originais da Manus;
- os arquivos originais `Untitled`;
- conteúdos das centrais privadas;
- caches operacionais;
- credenciais e configurações de acesso;
- logs internos;
- arquivos temporários;
- qualquer conteúdo privado ou ambíguo.

## Licenciamento

Fica aprovado o licenciamento duplo:

- MIT para scripts e códigos;
- CC BY 4.0 para dados derivados e documentação.

Os direitos do IBGE, da Manus e de quaisquer terceiros permanecem preservados.

## Manifesto

O núcleo publicável contém 20 arquivos validados pelo manifesto SHA-256.

```text
ARQUIVOS_NO_MANIFESTO=20
ARQUIVOS_APROVADOS=20
ARQUIVOS_REPROVADOS=0
RC_VALIDACAO=0
SHA256_MANIFESTO=73509ab035167ea8f7eeaa3e281ae1fcdb38eb71ff710df421781116713f0002

```

## Decisão

Considerando:

- a integridade dos arquivos;
- a equivalência dos hashes;
- a ausência de achados sensíveis;
- a documentação pública atualizada;
- a rastreabilidade registrada;
- o licenciamento definido;
- a validação integral do manifesto;

fica aprovado o pacote local GitHub sanitizado V1.0.

## Status formal

```text
APROVADO_PACOTE_GITHUB_SANITIZADO_V1_0
```

## Condição para publicação

A aprovação deste bloco limita-se à preparação local.

Continuam dependendo de autorização expressa do responsável:

- inicialização do repositório Git na pasta sanitizada;
- criação ou vinculação do repositório remoto;
- definição final do nome público;
- primeiro commit;
- push;
- alteração de visibilidade;
- divulgação pública.

## Estado operacional

```text
PACOTE_LOCAL_APROVADO=SIM
REPOSITORIO_GIT_INICIALIZADO=NAO
REMOTO_CONFIGURADO=NAO
COMMIT_REALIZADO=NAO
PUSH_REALIZADO=NAO
PUBLICACAO_REALIZADA=NAO
```

## Ratificação após recuperação R1

A validação final inicial identificou duas cercas Markdown não encerradas.

As duas ocorrências foram corrigidas no Bloco 18H-A-R1, sem alteração dos dados públicos ou do escopo aprovado.

O manifesto foi regenerado e seus 20 arquivos foram novamente aprovados, com código de retorno zero.

Hash vigente do manifesto:

`73509ab035167ea8f7eeaa3e281ae1fcdb38eb71ff710df421781116713f0002`

Fica ratificada a decisão:

`APROVADO_PACOTE_GITHUB_SANITIZADO_V1_0`