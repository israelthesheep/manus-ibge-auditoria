# Metodologia pública

## Objetivo

Avaliar a confiabilidade de duas entregas geradas pela Manus para indicadores municipais do IBGE, distinguindo correção dos valores, cobertura, estrutura, rastreabilidade e capacidade de uso analítico.

## Desenho do experimento

Foram comparadas duas execuções:

- **Rodada 01:** entrega inicial;
- **Rodada 02:** nova execução com orientação mais controlada.

A comparação está restrita a essas duas execuções e não constitui prova causal generalizável sobre todos os usos da ferramenta.

## Dimensões avaliadas

A pontuação considerou critérios relacionados a:

- compreensão e delimitação;
- extração e fonte;
- correção dos valores;
- cobertura;
- tratamento e modelagem;
- documentação;
- reprodutibilidade;
- publicação.

A correção dos valores foi avaliada separadamente da completude. Assim, uma entrega pode apresentar valores corretos nos registros materializados e ainda ser inadequada como produto analítico por falta de cobertura, estrutura ou documentação.

## Resultados

### Rodada 01

- pontuação: 57,13;
- classificação: `INSUFICIENTE_PARA_USO_ANALITICO`;
- cobertura de indicadores: 25%;
- cobertura funcional-temporal: 31,25%;
- condições bloqueadoras: 4.

### Rodada 02

- pontuação: 86,38;
- classificação numérica: `CONFIAVEL_NA_EXTENSAO_AUDITADA`;
- classificação global: `UTILIZAVEL_COM_RESSALVAS`;
- cobertura de indicadores: 75%;
- cobertura funcional-temporal: 68,75%;
- registros auditados: 61.273;
- divergências reais: 0;
- indicador ausente: área territorial.

## Produção dos derivados públicos

O dossiê técnico V1.0 foi encerrado e congelado com:

- 456 arquivos;
- 79.265.230 bytes;
- SHA-256 raiz:

`326ef01d169ebba93e6f100a354ef3fb554502e720cc98173118a3bfeb521e39`

A camada pública foi criada por derivação, sem alterar o dossiê técnico congelado.

Foram aplicados:

1. seleção de artefatos publicáveis;
2. remoção de caminhos e metadados operacionais sensíveis;
3. padronização de nomes e colunas;
4. inclusão de campos editoriais de proveniência;
5. geração e comparação de hashes;
6. QA dos derivados públicos;
7. revisão humana;
8. publicação analítica no Tableau.

## Categorias de informação

Os derivados distinguem:

- `ENTREGA_MANUS`;
- `AUDITORIA_INDEPENDENTE`;
- `DERIVADO_PUBLICACAO`;
- `INTERPRETACAO_EXPERIMENTAL`.

Essa separação evita apresentar interpretações da auditoria como se fossem informações produzidas pela ferramenta auditada.

## Controles de qualidade

O QA dos derivados públicos avaliou 25 controles:

- controles aprovados: 25;
- controles reprovados: 0;
- arquivos de dados avaliados: 7;
- registros granulares avaliados: 61.273;
- municípios na dimensão: 5.571.

Os hashes dos arquivos foram comparados entre a origem canônica, a publicação operacional para Tableau e o pacote normalizado do projeto.

## Publicação analítica

A etapa Tableau V1.0 foi concluída, revisada e publicada.

O painel público apresenta cinco telas:

1. Capa;
2. Painel Principal;
3. Extensão;
4. Rastrear;
5. Método.

A documentação e os links das Notas Técnicas estão disponíveis em `tableau/README.md`.

## Limites

- a área territorial não foi materializada na Rodada 02;
- a confiabilidade numérica vale somente para os registros efetivamente auditados;
- a cobertura incompleta impede uma classificação global irrestrita;
- a comparação de duas execuções não demonstra causalidade geral;
- o repositório público permite verificar os derivados, mas não regenerar o experimento desde as evidências brutas;
- o dossiê técnico congelado e os arquivos originais da Manus não são redistribuídos.

## Conclusão metodológica

A Rodada 02 apresentou melhoria substancial em relação à Rodada 01, especialmente na correção dos valores, na estrutura analítica e na cobertura.

Entretanto, a ausência de um dos indicadores esperados impede tratar a entrega como completa.

A conclusão consolidada é:

`MELHORIA_SUBSTANCIAL_COM_INCOMPLETUDE_REMANESCENTE`