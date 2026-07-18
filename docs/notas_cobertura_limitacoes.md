# Notas de cobertura e limitações

## Limitação principal

A área territorial não foi materializada pela Manus na Rodada 02.

## Classificação da Rodada 02

- valores entregues: `CONFIAVEL_NA_EXTENSAO_AUDITADA`;
- cobertura: `COBERTURA_INCOMPLETA`;
- classificação global: `UTILIZAVEL_COM_RESSALVAS`.

## Extensão validada

A auditoria da Rodada 02 alcançou:

- 61.273 registros;
- 5.571 municípios;
- 0 divergências reais nos registros materializados;
- 3 dos 4 indicadores esperados;
- 11 das 16 unidades indicador-período esperadas;
- cobertura de indicadores de 75%;
- cobertura funcional-temporal de 68,75%.

## Indicador ausente

O indicador de área territorial permaneceu ausente na Rodada 02.

Essa ausência impede classificar a entrega como completa, ainda que os valores efetivamente entregues tenham apresentado concordância na extensão auditada.

## Observações técnicas

No arquivo granular da Rodada 02:

- o campo `valor` possui 61.271 valores não nulos em 61.273 registros;
- o campo `unidade` não foi materializado;
- as unidades analíticas são descritas nos arquivos comparativos e de cobertura, quando aplicável;
- a classificação de confiabilidade não deve ser estendida a registros ou indicadores ausentes.

## Correção não equivale a completude

A ausência de divergências reais demonstra a qualidade dos valores materializados, mas não elimina limitações relacionadas a:

- cobertura;
- estrutura de publicação;
- documentação;
- rastreabilidade;
- indicadores não entregues.

Por isso, a classificação numérica e a classificação global são registradas separadamente.

## Comparação entre as rodadas

A Rodada 02 apresentou:

- aumento de 29,25 pontos na avaliação global;
- avanço de 50 pontos percentuais na cobertura de indicadores;
- avanço de 37,50 pontos percentuais na cobertura funcional-temporal;
- redução das condições bloqueadoras de 4 para 1.

A melhoria foi substancial, mas não eliminou a incompletude.

## Limite experimental

O experimento compara somente duas execuções.

Seus resultados:

- descrevem o comportamento observado neste projeto;
- não constituem prova causal generalizável;
- não devem ser aplicados automaticamente a outros prompts, agentes, bases ou contextos;
- não representam avaliação institucional do IBGE;
- não representam endosso ou certificação da Manus.

## Limite de reprodução pública

O repositório público permite verificar:

- os derivados sanitizados;
- os resultados comparativos;
- os hashes;
- a estrutura dos dados;
- a documentação metodológica.

O dossiê técnico congelado, as evidências brutas e os arquivos originais da Manus não são redistribuídos. Portanto, a reprodução pública começa nos derivados validados, e não nas evidências originais.

## Interpretação final

A Rodada 02 produziu valores confiáveis na extensão auditada e uma estrutura analítica consideravelmente superior à Rodada 01.

Entretanto, a cobertura permaneceu incompleta.

A conclusão correta é:

`MELHORIA_SUBSTANCIAL_COM_INCOMPLETUDE_REMANESCENTE`