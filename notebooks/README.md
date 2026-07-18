# Notebooks

A versão pública V1.0 não distribui notebooks dependentes do dossiê técnico congelado ou das evidências originais da Manus.

## Verificação pública

A integridade e a estrutura dos CSVs podem ser verificadas com o roteiro disponível em:

[`../docs/roteiro_reproducao.md`](../docs/roteiro_reproducao.md)

As verificações propostas utilizam apenas:

- Python 3;
- biblioteca padrão;
- arquivos públicos sanitizados;
- manifesto SHA-256.

## Limite de reprodução

O repositório público permite reproduzir verificações e análises a partir dos derivados validados.

Ele não permite reconstruir integralmente:

- as execuções originais da Manus;
- o dossiê técnico congelado;
- as evidências brutas;
- os caches operacionais;
- as etapas privadas de acesso.

## Inclusões futuras

Notebooks somente poderão ser incluídos após:

1. sanitização;
2. remoção de caminhos locais;
3. remoção de credenciais e metadados privados;
4. teste de reexecução;
5. revisão humana;
6. atualização do manifesto público;
7. nova decisão de publicação.