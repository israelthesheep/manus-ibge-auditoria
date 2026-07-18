# Política de Sanitização da Camada Pública — V1.0

## Princípio

A camada pública é derivada. O dossiê técnico congelado permanece imutável.

## Remoção ou revisão obrigatória

Devem ser removidos, substituídos ou explicitamente autorizados:

- caminhos locais Windows ou Git Bash;
- nomes de máquina, VDI ou estação;
- nomes de usuário internos;
- tokens, chaves, senhas e segredos;
- arquivos `.env`;
- arquivos `kaggle.json`;
- credenciais de APIs e serviços;
- identificadores privados de pastas e documentos;
- links não destinados ao público;
- endereços de e-mail não autorizados;
- metadados operacionais desnecessários;
- informações pessoais;
- comentários ou logs com contexto interno.

## Conteúdo técnico permitido

Podem ser publicados após validação:

- metodologia;
- métricas agregadas;
- matrizes comparativas;
- pontuações;
- conclusões;
- scripts sanitizados;
- dados públicos derivados;
- dicionários;
- manifestos públicos;
- hashes dos derivados;
- referência ao hash-raiz do dossiê.

## Quarentena

Arquivos binários, imagens, anexos ou conteúdos ambíguos deverão ser enviados
à quarentena até revisão humana.

## Regra de integridade

Cada derivado público deverá registrar:

- artefato de origem;
- versão de origem;
- hash de origem;
- transformações aplicadas;
- hash do derivado;
- destino pretendido;
- responsável pela revisão;
- decisão de publicação.
