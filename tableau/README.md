# Tableau Public

## Visualização

[Manus — Auditoria pública de uma IA](https://public.tableau.com/app/profile/israel.sheep/viz/Manus-AuditoriapblicadeIAv1_0/Capa?publish=yes)

A publicação possui cinco telas:

1. Capa;
2. Painel Principal;
3. Extensão;
4. Rastrear;
5. Método.

## Notas Técnicas

- [Tela 01 — Painel Principal](https://israelthesheep.vps-kinghost.net/html/manus/tela01_nota/)
- [Tela 02 — Extensão](https://israelthesheep.vps-kinghost.net/html/manus/tela02_nota/)
- [Tela 03 — Rastrear](https://israelthesheep.vps-kinghost.net/html/manus/tela03_nota/)
- [Tela 04 — Método](https://israelthesheep.vps-kinghost.net/html/manus/tela04_nota/)

## Fontes utilizadas

O Tableau consome os sete derivados públicos por meio da área operacional `datawarehouse` do Google Drive.

As cópias equivalentes e validadas por SHA-256 estão disponíveis na pasta `data/` deste repositório.

O Google Drive funciona como camada de distribuição. Ele não substitui:

- a origem canônica dos derivados;
- o dossiê técnico congelado;
- os registros de linhagem;
- os controles de integridade.

## Conteúdo das telas

### Capa

Apresenta o projeto, a pergunta de auditoria e a mensagem central.

### Painel Principal

Mostra o que foi entregue, o que permaneceu ausente e qual foi a extensão efetivamente auditada.

### Extensão

Compara literalmente as Rodadas 01 e 02, incluindo pontuação, cobertura, indicadores materializados e condições bloqueadoras.

### Rastrear

Explica o que foi validado, como os dados foram classificados e quais elementos sustentam a rastreabilidade pública.

### Método

Apresenta método, limites, interpretação correta e distinção entre confiabilidade dos valores e completude da entrega.

## Limite interpretativo

A visualização deve ser interpretada em conjunto com:

- as Notas Técnicas;
- `docs/metodologia.md`;
- `docs/notas_cobertura_limitacoes.md`;
- `docs/linhagem_publica.csv`.

A classificação `CONFIAVEL_NA_EXTENSAO_AUDITADA` não significa que a entrega esteja completa.

## Estado

```text
APROVADO_ENCERRAMENTO_ETAPA_TABLEAU_V1_0
```