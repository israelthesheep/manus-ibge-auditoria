# BLOCO 18J-A — Rascunho do artigo Medium V1.0

Projeto: **Manus × IBGE — Auditoria Pública de uma IA Agente**  
Projeto editorial: **Israel The Sheep**  
Responsável técnico e autor: **Igor Vasconcellos**  
Data do rascunho: **2026-07-20**  
Destino editorial: **Medium**  
Estado: **RASCUNHO — NÃO PUBLICAR**

## Controle editorial

- Título principal: **Dado correto não basta: uma auditoria pública de uma IA agente com dados do IBGE**
- Subtítulo principal: **Quando 61.273 registros sem divergências ainda não significam uma entrega completa**
- Mensagem central: **Dado correto não é sinônimo de entrega confiável. Sem cobertura, rastreabilidade, documentação e validação, até milhares de valores certos podem sustentar uma conclusão errada.**
- Versões incluídas: **longa e curta**
- Fonte de verdade para Kaggle, links e licenças: `REGISTRO_PUBLICACAO_KAGGLE_NOTEBOOKS_V1_0.md`
- Links pendentes: **Google Drive, GitHub e documentação pública**
- Publicação autorizada: **NÃO**

## Alternativas de título e subtítulo

### Alternativa 1

**Título:** Valores corretos, cobertura incompleta: o que aprendi auditando uma IA agente  
**Subtítulo:** Uma comparação em duas rodadas mostra por que exatidão, sozinha, não garante confiabilidade analítica

### Alternativa 2

**Título:** A diferença entre extrair dados e entregar dados confiáveis  
**Subtítulo:** Como uma auditoria com dados municipais do IBGE revelou melhora substancial — e incompletude remanescente

### Alternativa 3

**Título:** O que mudou quando o prompt mudou?  
**Subtítulo:** A mesma IA agente passou de 57,13 para 86,38 pontos, mas ainda exigiu ressalvas

---

# VERSÃO LONGA

# Dado correto não basta: uma auditoria pública de uma IA agente com dados do IBGE

## Quando 61.273 registros sem divergências ainda não significam uma entrega completa

Uma base com 61.273 registros auditados e nenhuma divergência real parece, à primeira vista, uma entrega plenamente confiável. Mas correção e completude não são a mesma coisa.

Neste experimento, auditei duas entregas da Manus sobre indicadores municipais do IBGE. A primeira recebeu 57,13 pontos e foi considerada insuficiente para uso analítico. Após a reformulação do prompt, a segunda alcançou 86,38 pontos — uma melhora substancial.

Mesmo assim, a classificação global permaneceu **utilizável com ressalvas**. Um dos indicadores solicitados não foi entregue, a cobertura ficou abaixo do escopo completo e a organização dos arquivos dificultou a rastreabilidade.

O resultado revelou a principal lição deste projeto: **dado correto não é sinônimo de entrega confiável. Sem cobertura, rastreabilidade, documentação e validação, até milhares de valores certos podem sustentar uma conclusão errada.**

[INSERIR IMAGEM 01 — banner ou capa do projeto]

*Legenda sugerida: Manus × IBGE — auditoria pública de uma IA agente, projeto Israel The Sheep.*

## Por que auditar uma IA agente?

Uma IA agente não apenas produz uma resposta em texto. Dependendo da tarefa, ela pode navegar por sites, localizar fontes, baixar arquivos, organizar dados, executar transformações e apresentar uma conclusão.

Essa autonomia muda a natureza da verificação. Quando o sistema declara que concluiu uma tarefa, o resultado visível nem sempre revela o que ficou ausente durante a execução.

Em uma resposta curta, um erro pode aparecer em uma frase. Em uma entrega de dados, os problemas podem assumir formas menos evidentes:

- um indicador solicitado pode não ter sido entregue;
- determinado período pode estar incompleto;
- uma tabela pode conter valores corretos, mas sem origem identificável;
- arquivos podem ser publicados com nomes genéricos;
- a conclusão pode declarar sucesso completo mesmo quando apenas parte do escopo foi atendida.

Auditar não significa partir do pressuposto de que a IA está errada. Significa exigir que o resultado possa ser verificado por outra pessoa.

Por isso, este projeto não tratou “valor correto” como sinônimo de “trabalho concluído”. A entrega foi examinada como um produto de dados: conteúdo, cobertura, organização, documentação, rastreabilidade, possibilidade de reprodução e limites de uso.

O experimento também não pretende avaliar toda a Manus nem generalizar suas conclusões para todas as IAs agentes. Ele examina duas entregas específicas, dentro de um escopo definido e comparadas com referências públicas do IBGE.

## O problema proposto

A solicitação feita à Manus parecia simples: localizar e organizar um conjunto de indicadores municipais publicados pelo IBGE.

Na prática, a tarefa envolvia mais do que encontrar números. Para que a entrega pudesse ser utilizada em uma análise, ela precisava:

1. identificar as fontes correspondentes aos indicadores solicitados;
2. entregar os municípios e períodos previstos;
3. preservar a relação entre os valores e suas origens;
4. organizar os dados em arquivos compreensíveis;
5. documentar o método, o conteúdo e as limitações;
6. permitir que outra pessoa verificasse os resultados.

O verdadeiro teste, portanto, não era saber se a Manus conseguiria encontrar dados do IBGE. Era verificar se ela conseguiria transformar esses dados em uma entrega analítica completa, rastreável e validável.

O experimento foi realizado em duas rodadas. A primeira utilizou a solicitação original. Na segunda, o prompt foi reformulado, mantendo o mesmo objetivo analítico.

Essa comparação permitiu observar duas coisas: quanto a formulação do pedido influencia o desempenho de uma IA agente e até onde um prompt melhor consegue resolver os problemas encontrados na primeira entrega.

O critério de sucesso não foi a quantidade de linhas produzidas nem a declaração de que a tarefa havia sido concluída. O resultado precisava corresponder ao escopo solicitado e apresentar evidências suficientes para sustentar essa conclusão.

## Como a auditoria foi conduzida

A auditoria começou pela preservação das entregas originais. Os arquivos recebidos foram mantidos sem alteração, enquanto as verificações e os materiais públicos foram produzidos em camadas separadas.

Em cada rodada, os dados entregues pela Manus foram comparados com referências públicas do IBGE dentro de um escopo previamente definido. A análise separou dimensões que poderiam ser confundidas se observadas apenas pela pontuação final:

- **correção dos valores:** verificou se os registros existentes coincidiam com a referência auditada;
- **cobertura de indicadores:** mediu quanto do conjunto solicitado foi efetivamente entregue;
- **cobertura funcional e temporal:** avaliou o atendimento combinado às funções e aos períodos previstos;
- **rastreabilidade:** examinou se era possível identificar a origem dos dados e acompanhar o percurso da entrega;
- **documentação:** verificou se método, conteúdo e limitações estavam explicados;
- **organização da publicação:** avaliou se os arquivos podiam ser identificados e utilizados com segurança;
- **reprodutibilidade:** observou se outra pessoa conseguiria repetir as verificações com os artefatos disponíveis.

Separar correção e cobertura foi uma decisão essencial. Um indicador ausente não gera necessariamente uma divergência de valor, porque não existe registro para comparar. Se apenas os dados presentes fossem avaliados, a ausência poderia desaparecer da conclusão.

A pontuação sintetizou o desempenho da entrega dentro desse protocolo, mas não foi utilizada isoladamente. Cobertura, bloqueios críticos e limites da evidência também participaram da interpretação global.

Por isso, a Rodada 02 pôde alcançar 86,38 pontos e ser considerada confiável na extensão auditada, enquanto a conclusão global permaneceu **utilizável com ressalvas**.

A diferença entre essas duas classificações protege a leitura dos resultados: a primeira descreve a qualidade do que foi efetivamente validado; a segunda considera se a entrega completa atendeu ao que havia sido solicitado.

## Rodada 01: valores presentes não compensaram a baixa cobertura

A primeira rodada terminou com **57,13 pontos** e foi classificada como **insuficiente para uso analítico**.

Os principais resultados foram:

- cobertura de indicadores: **25%**;
- cobertura funcional e temporal: **31,25%**;
- bloqueios críticos: **4**;
- duração observada: **19 minutos**;
- créditos consumidos: **524**.

A cobertura de 25% mostra que três quartos do escopo de indicadores permaneceram sem atendimento. Na dimensão funcional e temporal, menos de um terço do que estava previsto foi efetivamente coberto.

Os quatro bloqueios críticos reforçaram que não se tratava de uma pequena diferença de acabamento. A entrega não oferecia condições suficientes para sustentar uso analítico seguro dentro do escopo solicitado.

Isso não significa que todos os valores presentes estavam errados. O problema principal estava na distância entre o conteúdo entregue e aquilo que deveria ter sido entregue.

Uma tabela pode transmitir sensação de abundância porque contém muitas linhas. Mas quantidade de registros não mede completude. Quando partes relevantes do escopo estão ausentes, uma análise posterior pode parecer consistente e ainda assim responder a uma pergunta diferente da original.

A duração de 19 minutos e o consumo de 524 créditos descrevem essa execução específica. Esses números serão úteis na comparação com a Rodada 02, mas não devem ser interpretados isoladamente como uma medida universal de eficiência.

A Rodada 01 estabeleceu, portanto, a linha de base do experimento: havia conteúdo aproveitável, mas cobertura e bloqueios impediam que a entrega fosse considerada adequada para uso analítico.

## Rodada 02: melhora substancial, com uma ressalva decisiva

Com o prompt reformulado, a segunda rodada alcançou **86,38 pontos**. A classificação numérica foi **confiável na extensão auditada**, enquanto a classificação global ficou em **utilizável com ressalvas**.

A comparação mostra uma mudança expressiva:

| Métrica | Rodada 01 | Rodada 02 | Diferença |
| --- | ---: | ---: | ---: |
| Pontuação | 57,13 | 86,38 | +29,25 pontos |
| Cobertura de indicadores | 25% | 75% | +50 pontos percentuais |
| Cobertura funcional e temporal | 31,25% | 68,75% | +37,50 pontos percentuais |
| Duração observada | 19 min | 10 min | −9 min |
| Créditos consumidos | 524 | 380 | −144 |

A pontuação aumentou **51,20%** em relação à primeira rodada. No experimento, essa melhora ocorreu junto com uma execução mais curta e menor consumo de créditos. Ainda assim, duração e créditos são medidas descritivas das duas execuções, não uma garantia de que o mesmo comportamento se repetirá em outros contextos.

> **Nota sobre créditos:** “créditos” são a unidade de consumo registrada pela própria Manus. Não equivalem diretamente a reais, tokens de API ou uma medida universal de custo. A segunda rodada consumiu 144 créditos a menos — redução observada de 27,48% —, mas o dado deve ser interpretado apenas dentro destas duas execuções.

O resultado mais importante veio da validação dos dados. A auditoria examinou **61.273 registros**, cobrindo **5.571 municípios**, e encontrou **zero divergências reais nos valores existentes**, dentro da extensão auditada.

Esse resultado demonstra que os dados efetivamente presentes se mostraram confiáveis no recorte verificado. Mas a extensão validada ainda não correspondia ao escopo completo solicitado.

O indicador **área territorial** permaneceu ausente. A cobertura de indicadores chegou a 75%, não a 100%, e a cobertura funcional e temporal alcançou 68,75%.

Por isso, a segunda rodada não foi classificada como perfeita ou plenamente completa. A formulação tecnicamente adequada foi:

> **Melhoria substancial com incompletude remanescente.**

Os valores existentes passaram pela validação. A entrega completa, porém, ainda exigia ressalvas.

[INSERIR IMAGEM 02 — comparação visual das duas rodadas]

*Legenda sugerida: A pontuação cresceu 29,25 pontos, enquanto a cobertura permaneceu abaixo do escopo integral.*

## O que mudou quando o prompt mudou

A comparação entre as rodadas mostra que a formulação do pedido influencia de maneira concreta o desempenho de uma IA agente.

Na segunda execução, o objetivo analítico foi mantido, mas o prompt foi reformulado para tornar o escopo e os requisitos da entrega mais explícitos. O resultado melhorou em várias dimensões ao mesmo tempo: pontuação, cobertura de indicadores, cobertura funcional e temporal, duração observada e consumo de créditos.

Isso não significa que todos os ganhos possam ser atribuídos exclusivamente ao prompt. As duas rodadas não constituem um experimento controlado capaz de isolar cada variável envolvida na execução. A conclusão válida é mais restrita: **dentro deste experimento, o prompt reformulado foi acompanhado por uma melhora substancial da entrega**.

Ao mesmo tempo, o indicador ausente demonstra que um prompt melhor não elimina a necessidade de auditoria. A reformulação reduziu problemas importantes, mas não garantiu o atendimento integral do escopo.

O experimento sugere uma divisão clara de responsabilidades:

- o prompt estabelece o contrato esperado;
- a IA executa a tarefa;
- a auditoria verifica se o contrato foi cumprido;
- a governança define o que pode ser utilizado ou publicado e quais ressalvas precisam acompanhar o resultado.

A qualidade do prompt importa, mas ela não substitui cobertura mensurável, rastreabilidade, documentação e validação independente.

**Não basta pedir melhor. É preciso conferir melhor.**

## Zero divergências não significa entrega completa

Os resultados da Rodada 02 respondem a perguntas diferentes, e elas não devem ser misturadas:

| Pergunta | Evidência utilizada | Resultado |
| --- | --- | ---: |
| Os valores existentes coincidem com a referência auditada? | Divergências reais | **0** |
| Todos os indicadores solicitados foram entregues? | Cobertura de indicadores | **75%** |
| Funções e períodos previstos foram atendidos integralmente? | Cobertura funcional e temporal | **68,75%** |

A ausência de divergências demonstra a qualidade dos valores que existiam e puderam ser comparados. Ela não mede aquilo que deixou de ser entregue.

Quando um indicador está ausente, não há um valor incorreto para identificar — não há valor algum. Se cobertura e correção forem tratadas como a mesma dimensão, essa ausência desaparece da avaliação.

Por isso, “zero divergências reais” não significa:

- que todos os indicadores solicitados foram entregues;
- que todos os períodos e funções estavam cobertos;
- que qualquer conclusão poderia ser generalizada;
- que futuras execuções produzirão o mesmo resultado;
- que todas as capacidades da Manus foram validadas.

A formulação tecnicamente precisa é mais restrita:

> **Nos 61.273 registros existentes e comparados dentro da extensão auditada, não foram encontradas divergências reais.**

Essa frase reconhece um resultado muito positivo sem ultrapassar os limites da evidência.

Os valores presentes eram confiáveis no recorte examinado. A cobertura, porém, continuava incompleta. É justamente essa diferença que impede milhares de valores corretos de se transformarem, por engano, em uma declaração de sucesso integral.

## O problema dos arquivos `Untitled`

A organização dos arquivos também fez parte da auditoria. Na entrega original, alguns artefatos foram publicados com nomes genéricos como `Untitled`, dificultando a identificação do conteúdo e a reconstrução do percurso da entrega.

Isso não significa que os valores desses arquivos estavam necessariamente errados. O problema era de organização, uso e rastreabilidade.

Em um produto de dados, o nome do arquivo funciona como metadado. Ele deveria ajudar a responder perguntas básicas:

- qual é o conteúdo do arquivo;
- a qual indicador ou etapa ele pertence;
- qual é sua versão;
- como ele se relaciona com os demais artefatos;
- se é uma evidência original ou um derivado preparado posteriormente.

Nomes genéricos aumentam o risco de utilização do arquivo errado, dificultam a associação entre dados e documentação e tornam a reprodução da análise mais dependente de conhecimento informal.

Para preservar a evidência, os arquivos originais não foram sobrescritos nem reorganizados como se tivessem sido entregues de outra forma. Eles foram mantidos separadamente em `originais_manus`.

Os derivados utilizados na camada pública foram preparados em outra estrutura, com nomes compreensíveis, documentação, validação e rastreabilidade próprias.

Essa separação permitiu manter duas funções distintas:

- **originais:** registrar exatamente o que foi recebido;
- **derivados públicos:** oferecer uma camada segura e compreensível para análise e reprodução.

Organização não corrige valores, mas interfere diretamente na confiabilidade operacional de uma entrega. Um arquivo pode estar matematicamente correto e, ainda assim, ser difícil de localizar, interpretar ou relacionar com sua origem.

Por isso, o problema dos arquivos `Untitled` não foi tratado como detalhe estético. Ele foi registrado como uma limitação de publicação e governança.

## O que o Tableau mostra

Os resultados da auditoria foram organizados em uma visualização pública no Tableau. O objetivo foi transformar o dossiê técnico em uma leitura acessível sem reduzir toda a análise a uma única pontuação.

Os painéis conduzem o leitor por quatro perspectivas complementares:

- **escopo principal:** mostra o que era esperado, o que foi entregue, o que permaneceu ausente e qual foi a extensão efetivamente auditada;
- **comparação das rodadas:** apresenta lado a lado pontuação, cobertura, duração e créditos das Rodadas 01 e 02;
- **rastreio:** explica o que foi validado, quais evidências sustentam os resultados e onde terminam os limites da auditoria;
- **metodologia:** apresenta os critérios utilizados e orienta a interpretação das classificações.

Essa estrutura evita que a pontuação de 86,38 seja observada isoladamente. O leitor pode acompanhar a melhora da segunda rodada e, ao mesmo tempo, verificar a cobertura incompleta e o indicador ausente.

O Tableau funciona como uma porta de entrada visual para o projeto. Ele não substitui os dados, os notebooks ou a documentação técnica. As telas resumem os resultados, enquanto os demais artefatos permitem aprofundar e reproduzir as verificações.

A visualização está disponível em:

**[Acessar o Tableau público](https://public.tableau.com/app/profile/israel.sheep/viz/Manus-AuditoriapblicadeIAv1_0/Capa?publish=yes)**

[INSERIR CAPTURA DO TABLEAU]

*Legenda sugerida: A visualização separa pontuação, cobertura, rastreio e metodologia para impedir que uma única métrica conte toda a história.*

## Dados, notebooks e reprodutibilidade

Se o Tableau oferece a leitura visual, o Kaggle reúne os artefatos necessários para explorar e reproduzir as principais verificações do projeto.

O [dataset público Manus × IBGE](https://www.kaggle.com/datasets/israelthesheep/manus-ibge-auditoria-publica-de-ia) contém somente derivados públicos validados. Evidências originais da Manus, credenciais, arquivos privados e componentes da camada técnica congelada não foram incluídos.

O conjunto recebeu **Usability Score 10,00** no Kaggle. Essa nota indica que o dataset foi publicado com boa estrutura, descrição de arquivos, documentação de colunas e demais elementos esperados pela plataforma. Ela não substitui a validação analítica dos dados.

Três notebooks públicos apresentam diferentes perspectivas da auditoria:

1. **[Visão Geral da Auditoria Manus × IBGE](https://www.kaggle.com/code/israelthesheep/01-vis-o-geral-da-auditoria-manus-ibge)** — introduz o conjunto de dados e os principais resultados;
2. **[Validação de Cobertura da Rodada 02](https://www.kaggle.com/code/israelthesheep/02-valida-o-de-cobertura-da-rodada-02)** — examina indicadores, cobertura e ausências;
3. **[Comparação das Rodadas 01 e 02](https://www.kaggle.com/code/israelthesheep/03-compara-o-das-rodadas-01-e-02)** — apresenta a evolução entre as duas execuções.

Os três notebooks foram executados, versionados e confirmados como acessíveis publicamente sem autenticação.

Os dados e a documentação estão disponíveis sob licença **CC BY 4.0**. O código original dos notebooks permanece sob licença **MIT**, enquanto as versões publicadas no Kaggle Code também utilizam **Apache 2.0**, em regime de licenciamento duplo autorizado.

No encerramento técnico, o contador da aba de código do dataset ainda exibia zero, apesar de os três notebooks estarem públicos e utilizarem o conjunto como entrada. Essa diferença foi registrada como uma pendência de indexação da interface, não bloqueante. Ela não altera os dados, os notebooks ou os resultados da auditoria.

Publicar os artefatos não torna a análise automaticamente reproduzível. A reprodutibilidade depende da combinação entre dados compreensíveis, código executável, documentação, licenças claras e limites explicitados. Foi essa combinação que a camada pública procurou oferecer.

## Limites do experimento

Toda auditoria responsável precisa declarar onde suas conclusões terminam.

Este experimento avaliou duas entregas específicas da Manus, produzidas a partir de dois prompts e examinadas dentro de um escopo definido de indicadores municipais do IBGE.

Os resultados não permitem concluir que:

- toda entrega da Manus terá o mesmo comportamento;
- todas as IAs agentes apresentam os mesmos problemas;
- futuras execuções repetirão os resultados observados;
- os valores não examinados pela auditoria também estão corretos;
- a melhora entre as rodadas foi causada exclusivamente pela reformulação do prompt;
- duração e créditos representam um benchmark universal de desempenho.

A auditoria também não procurou inferir intenção, explicar o funcionamento interno da plataforma ou determinar por que determinado indicador deixou de ser entregue. Ela avaliou os artefatos recebidos e as evidências que puderam ser verificadas.

A ausência de divergências é válida somente para os registros comparados dentro da extensão auditada. Da mesma forma, as medições de tempo e créditos descrevem aquelas duas execuções, sujeitas às condições do ambiente e da plataforma.

Os dados públicos do IBGE e as próprias ferramentas envolvidas podem ser atualizados ao longo do tempo. Os resultados deste projeto correspondem às versões, arquivos e referências preservados no dossiê técnico.

Esse dossiê foi congelado antes da preparação da camada pública. A organização posterior dos derivados, a publicação no Google Drive, no Tableau e no Kaggle e a criação deste artigo não modificaram os resultados analíticos originais.

Portanto, a conclusão deve permanecer vinculada à formulação correta:

> **Na entrega auditada, houve melhora substancial, os valores existentes foram confiáveis na extensão examinada e a cobertura permaneceu incompleta.**

Esses limites não enfraquecem o experimento. Eles definem exatamente o que suas evidências conseguem sustentar.

## Conclusão: confiança precisa de fronteiras

Entre “a IA acertou” e “a IA falhou”, a auditoria encontrou uma resposta mais útil: **a Manus entregou valores confiáveis no recorte validado, mas não entregou todo o escopo solicitado**.

A primeira rodada, com 57,13 pontos, não apresentou condições suficientes para uso analítico. A segunda alcançou 86,38 pontos, ampliou a cobertura e produziu 61.273 registros sem divergências reais nos valores existentes.

A melhora foi substancial. A incompletude também foi real.

O indicador de área territorial continuou ausente, a cobertura de indicadores permaneceu em 75% e a cobertura funcional e temporal chegou a 68,75%. Por isso, a conclusão não poderia ser “resultado perfeito”, da mesma forma que os avanços impediam classificá-la simplesmente como fracasso.

A formulação mais fiel às evidências foi:

> **Melhoria substancial com incompletude remanescente.**

O experimento mostra que IAs agentes podem acelerar a localização, a organização e o tratamento de dados. Mas essa capacidade também pode ampliar rapidamente uma entrega incompleta se volume e aparência de precisão forem confundidos com confiabilidade.

É nesse ponto que a governança deixa de ser um complemento burocrático. Cobertura mensurável, preservação dos originais, rastreabilidade, documentação, validação independente e limites explícitos são o que transforma uma saída automatizada em um produto de dados defensável.

Confiar na extensão auditada não significa confiar sem fronteiras. Significa saber exatamente o que foi validado, o que ficou ausente e até onde a conclusão pode ser utilizada.

**O dado certo é indispensável. Só não é o trabalho inteiro.**

## Recursos públicos

- **Tableau:** [painel público](https://public.tableau.com/app/profile/israel.sheep/viz/Manus-AuditoriapblicadeIAv1_0/Capa?publish=yes)
- **Kaggle:** [dataset público](https://www.kaggle.com/datasets/israelthesheep/manus-ibge-auditoria-publica-de-ia)
- **Notebook 01:** [visão geral da auditoria](https://www.kaggle.com/code/israelthesheep/01-vis-o-geral-da-auditoria-manus-ibge)
- **Notebook 02:** [validação de cobertura da Rodada 02](https://www.kaggle.com/code/israelthesheep/02-valida-o-de-cobertura-da-rodada-02)
- **Notebook 03:** [comparação das Rodadas 01 e 02](https://www.kaggle.com/code/israelthesheep/03-compara-o-das-rodadas-01-e-02)
- **Google Drive:** [entrega original preservada](https://drive.google.com/drive/folders/1tWWK0ZvL-U7tadCOgWDr_r5U9OMwChJc)
- **GitHub:** [repositório público e documentação](https://github.com/israelthesheep/manus-ibge-auditoria)

---

# VERSÃO CURTA

# Dado correto não basta: uma auditoria pública de uma IA agente com dados do IBGE

## Quando 61.273 registros sem divergências ainda não significam uma entrega completa

Uma tabela pode conter milhares de valores corretos e, mesmo assim, não constituir uma entrega confiável. Isso acontece quando faltam cobertura, rastreabilidade, documentação ou condições para que outra pessoa valide o resultado.

Foi essa a questão central do projeto **Manus × IBGE — Auditoria Pública de uma IA Agente**. Em duas rodadas, uma entrega da Manus sobre indicadores municipais do IBGE foi avaliada não apenas pela exatidão dos valores, mas também como produto de dados.

Na **Rodada 01**, a entrega recebeu **57,13 pontos** e foi classificada como **insuficiente para uso analítico**. A cobertura de indicadores foi de apenas **25%**, a cobertura funcional e temporal chegou a **31,25%** e quatro bloqueios críticos foram identificados.

Após a reformulação do prompt, a **Rodada 02** alcançou **86,38 pontos** — um aumento de **29,25 pontos**, ou **51,20%**. A cobertura de indicadores subiu para **75%** e a cobertura funcional e temporal para **68,75%**.

A melhora não foi apenas numérica. A execução observada passou de 19 para 10 minutos, enquanto o consumo caiu de 524 para 380 créditos. Esses números descrevem o experimento e não devem ser tratados como benchmark universal.

Nesse contexto, “créditos” são a unidade de consumo registrada pela Manus. Eles não equivalem diretamente a dinheiro, tokens de API ou uma medida universal de custo. A redução observada foi de 144 créditos, ou 27,48%, entre as duas execuções.

O resultado mais forte veio da validação dos dados: **61.273 registros auditados e zero divergências reais nos valores existentes**, dentro da extensão examinada.

Então por que a classificação global ainda foi **utilizável com ressalvas**?

Porque correção e completude são dimensões diferentes. O indicador **área territorial** permaneceu ausente. A entrega melhorou muito, mas não cobriu todo o escopo solicitado. Dizer apenas que “não houve divergências” esconderia a parte que faltou.

Essa distinção é o centro da auditoria:

> **Dado correto não é sinônimo de entrega confiável. Sem cobertura, rastreabilidade, documentação e validação, até milhares de valores certos podem sustentar uma conclusão errada.**

A organização dos artefatos também importou. A publicação original apresentou arquivos com nomes genéricos como `Untitled`, dificultando a identificação do conteúdo e o rastreio da entrega. Para preservar a evidência, os originais foram mantidos em `originais_manus`, separados dos derivados públicos preparados para análise.

O projeto disponibiliza uma leitura visual no [Tableau](https://public.tableau.com/app/profile/israel.sheep/viz/Manus-AuditoriapblicadeIAv1_0/Capa?publish=yes), além de um [dataset público no Kaggle](https://www.kaggle.com/datasets/israelthesheep/manus-ibge-auditoria-publica-de-ia) e três notebooks sobre visão geral, cobertura da Rodada 02 e comparação entre as rodadas.

A conclusão não é que a Manus “acertou tudo” nem que “falhou por completo”. A formulação tecnicamente honesta é: **melhoria substancial com incompletude remanescente**.

Na extensão auditada, os valores existentes foram confiáveis. No conjunto, a entrega exigiu ressalvas. É exatamente por isso que IAs agentes precisam de governança: critérios explícitos, preservação dos originais, cobertura mensurável, documentação, rastreabilidade e validação independente.

O dado certo é indispensável. Só não é o trabalho inteiro.

## Recursos públicos

- [Tableau público](https://public.tableau.com/app/profile/israel.sheep/viz/Manus-AuditoriapblicadeIAv1_0/Capa?publish=yes)
- [Dataset no Kaggle](https://www.kaggle.com/datasets/israelthesheep/manus-ibge-auditoria-publica-de-ia)
- [Notebook 01 — Visão geral](https://www.kaggle.com/code/israelthesheep/01-vis-o-geral-da-auditoria-manus-ibge)
- [Notebook 02 — Cobertura da Rodada 02](https://www.kaggle.com/code/israelthesheep/02-valida-o-de-cobertura-da-rodada-02)
- [Notebook 03 — Comparação das rodadas](https://www.kaggle.com/code/israelthesheep/03-compara-o-das-rodadas-01-e-02)
- [Google Drive — entrega original preservada](https://drive.google.com/drive/folders/1tWWK0ZvL-U7tadCOgWDr_r5U9OMwChJc)
- [GitHub — repositório público e documentação](https://github.com/israelthesheep/manus-ibge-auditoria)

---

# CHECKLIST EDITORIAL

## 1. Validação técnica e factual

- [ ] Confirmar `PONTUACAO_R1=57,13`.
- [ ] Confirmar `PONTUACAO_R2=86,38`.
- [ ] Confirmar diferença de **29,25 pontos** e variação relativa de **51,20%**.
- [ ] Confirmar cobertura de indicadores: **25% → 75%**.
- [ ] Confirmar cobertura funcional e temporal: **31,25% → 68,75%**.
- [ ] Confirmar **quatro bloqueios críticos** na Rodada 01.
- [ ] Confirmar **61.273 registros auditados** na Rodada 02.
- [ ] Confirmar **zero divergências reais na extensão auditada**.
- [ ] Confirmar indicador ausente: **área territorial**.
- [ ] Confirmar duração: **19 min → 10 min**.
- [ ] Confirmar créditos: **524 → 380**.
- [ ] Manter separadas as formulações **“confiável na extensão auditada”** e **“utilizável com ressalvas”**.
- [ ] Não transformar ausência de divergência em alegação de cobertura total.
- [ ] Não alterar nem recalcular resultados do dossiê técnico congelado.

## 2. Links e publicação pública

- [x] Validar URL pública do Tableau.
- [x] Validar URL canônica do dataset Kaggle com slug `manus-ibge-auditoria-publica-de-ia`.
- [x] Validar links dos três notebooks Kaggle.
- [x] Substituir `[LINK_GOOGLE_DRIVE]` pelo link público definitivo.
- [x] Substituir `[LINK_GITHUB]` pelo link público definitivo.
- [x] Substituir `[LINK_DOCUMENTACAO_PUBLICA]` pelo GitHub ou remover o item redundante.
- [ ] Testar todos os links em janela anônima antes da publicação.
- [ ] Manter `CODE_DATASET=0` apenas como nota operacional, se ainda for editorialmente relevante.
- [ ] Não criar outro dataset nem republicar o pacote por causa do contador de código.

## 3. Licenças e atribuição

- [x] Dados e documentação: **CC BY 4.0**.
- [x] Código original dos notebooks: **MIT**.
- [x] Versões no Kaggle Code: **Apache 2.0**.
- [x] Licenciamento duplo: **autorizado e registrado**.
- [ ] Verificar se o Medium exige alguma nota adicional de atribuição nas imagens ou capturas.
- [ ] Identificar claramente Igor Vasconcellos como responsável técnico e autor.
- [ ] Mencionar Israel The Sheep como projeto editorial, sem converter o artigo em peça promocional.

## 4. Imagens e legibilidade

- [ ] Inserir banner/capa do projeto após a abertura.
- [ ] Inserir comparação visual das Rodadas 01 e 02.
- [ ] Inserir captura final do Tableau.
- [ ] Escrever texto alternativo descritivo para cada imagem.
- [ ] Conferir legibilidade em desktop e celular.
- [ ] Evitar imagens com números desatualizados ou simulados.
- [ ] Confirmar que as imagens não expõem caminhos locais, dados privados ou credenciais.

## 5. Revisão de tom e rigor

- [ ] Evitar acusação de mentira, fraude ou intenção não demonstrada.
- [ ] Evitar generalizações sobre a Manus ou sobre todas as IAs agentes.
- [ ] Evitar “resultado perfeito”, “IA inútil” e formulações sensacionalistas.
- [ ] Preservar a frase “a entrega declarou sucesso completo, mas a auditoria encontrou incompletude”, somente se a evidência pública sustentar a declaração de sucesso completo.
- [ ] Preferir “valores existentes” e “na extensão auditada”.
- [ ] Explicar que nomes `Untitled` afetam organização e rastreabilidade, não a correção matemática dos valores.
- [ ] Manter os limites do experimento visíveis antes da conclusão.
- [ ] Realizar revisão ortográfica e padronizar vírgula decimal em português.

## 6. SEO e apresentação no Medium

- [x] Definir título final e subtítulo final.
- [ ] Preparar descrição curta de compartilhamento, entre 140 e 160 caracteres.
- [ ] Selecionar até cinco tags coerentes, por exemplo: `Inteligência Artificial`, `Ciência de Dados`, `Governança de Dados`, `IBGE`, `Auditoria`.
- [ ] Escolher imagem de capa com crédito e texto alternativo.
- [ ] Conferir se a tabela comparativa renderiza bem; converter em imagem apenas se necessário.
- [ ] Inserir separadores com moderação.
- [ ] Fazer leitura final sem os títulos internos de controle deste arquivo.

## 7. Gate de publicação

- [ ] Escolher entre a versão longa e a versão curta; não publicar ambas como se fossem artigos independentes sem decisão editorial.
- [ ] Remover instruções entre colchetes e placeholders de imagens.
- [ ] Resolver ou remover todos os links pendentes.
- [ ] Registrar aprovação humana explícita do texto final.
- [ ] Publicar somente após confirmação expressa de Igor Vasconcellos.
- [ ] Registrar URL, data e versão do artigo publicado em artefato próprio.

## Status do bloco

```text
BLOCO=18J-A
ARTEFATO=RASCUNHO_ARTIGO_MEDIUM_V1_0.md
VERSAO_LONGA=CRIADA
VERSAO_CURTA=CRIADA
CHECKLIST_EDITORIAL=CRIADO
LINK_TABLEAU=VALIDADO_PELA_FONTE_DE_VERDADE
LINK_KAGGLE_DATASET=VALIDADO_PELA_FONTE_DE_VERDADE
LINKS_NOTEBOOKS_KAGGLE=3/3_VALIDOS_NA_FONTE_DE_VERDADE
TITULO_SUBTITULO=APROVADOS
ABERTURA_VERSAO_LONGA=APROVADA
SECAO_POR_QUE_AUDITAR=APROVADA
SECAO_PROBLEMA_PROPOSTO=APROVADA
SECAO_COMO_AUDITORIA_FOI_CONDUZIDA=APROVADA
SECAO_RODADA_01=APROVADA
SECAO_RODADA_02=APROVADA
SECAO_O_QUE_MUDOU_COM_O_PROMPT=APROVADA
SECAO_ZERO_DIVERGENCIAS_NAO_SIGNIFICA_COMPLETUDE=APROVADA
SECAO_ARQUIVOS_UNTITLED=APROVADA
SECAO_TABLEAU=APROVADA
SECAO_DADOS_NOTEBOOKS_REPRODUTIBILIDADE=APROVADA
SECAO_LIMITES_DO_EXPERIMENTO=APROVADA
SECAO_CONCLUSAO=APROVADA
NOTA_SOBRE_CREDITOS=INCLUIDA_AGUARDANDO_APROVACAO
LINK_GOOGLE_DRIVE=CONFIRMADO
LINK_GITHUB=CONFIRMADO_PELO_RESPONSAVEL_TECNICO
LINK_DOCUMENTACAO_PUBLICA=INCORPORADO_AO_GITHUB
DOSSIÊ_TECNICO_ALTERADO=NAO
ARTIGO_PUBLICADO=NAO
STATUS_ATUAL=RASCUNHO_GERADO_AGUARDANDO_REVISAO_E_APROVACAO
STATUS_ALVO=APROVADO_RASCUNHO_ARTIGO_MEDIUM_V1_0
```