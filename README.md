# Template para projetos de deeptech em saúde

**Uma estrutura para transformar uma ideia em um projeto científico e tecnológico que outras pessoas consigam examinar, discutir e desenvolver.**

Este repositório é para equipes que trabalham com software, inteligência artificial, dispositivos, diagnóstico, biotecnologia ou pesquisa translacional em saúde. Ele ajuda a organizar perguntas que costumam ficar dispersas entre apresentações, artigos, planilhas e conversas: qual problema será resolvido, que evidência o sustenta, o que será construído, como será testado e o que ainda depende de confirmação.

O resultado esperado é um conjunto de documentos conectados que torna visíveis as hipóteses, decisões, fontes, limites e próximas entregas de **um projeto por repositório**. Essa base pode apoiar a colaboração da equipe, a conversa com pesquisadores e instituições e a preparação de materiais para parceiros ou oportunidades de fomento. Cada apresentação ou candidatura precisa ser adaptada ao seu público e às exigências vigentes.

## A lógica do template

Um projeto de saúde precisa ligar a promessa da tecnologia ao caminho para verificá-la. Por isso, a estrutura segue uma cadeia de perguntas:

**Problema → evidências → hipótese → método → dados ou materiais → tecnologia → validação → impacto.**

O [documento mestre](PROJECT.md) reúne essas decisões e liga as frentes. O [registro de decisões](DECISIONS.md) mostra por que o rumo mudou. O [status](STATUS.md) distingue trabalho planejado de entregas comprovadas. Assim, uma alegação apresentada no resumo pode ser rastreada até sua fonte, seu método e sua evidência de validação — ou ficar explicitamente marcada como hipótese.

| Frente | Decisão que ajuda a tomar | Documento inicial |
|---|---|---|
| Visão | Para quem existe a solução e qual problema importa? | [Brief](00_VISAO/brief.md) |
| Evidências | O que já se sabe e onde está a lacuna? | [Lacuna e estado da arte](01_EVIDENCIAS/lacuna.md) |
| Pesquisa | Qual hipótese será testada e por qual método? | [Protocolo](02_PESQUISA/protocolo.md) |
| Dados | As fontes ou materiais são adequados e utilizáveis? | [Viabilidade e governança](03_DADOS/viabilidade.md) |
| Tecnologia | Como a solução será construída e reproduzida? | [Arquitetura](04_TECNOLOGIA/arquitetura.md) |
| Validação | Que comparação e quais métricas sustentariam a proposta? | [Plano de validação](05_VALIDACAO/plano.md) |
| Produto | Qual é o uso pretendido e o caminho para adoção? | [Estratégia](06_PRODUTO/estrategia.md) |
| Execução | Quais entregas, dependências e riscos vêm a seguir? | [Plano de execução](07_EXECUCAO/plano.md) |

A [matriz de referências](08_REFERENCIAS/matriz.md) dá lastro às afirmações; os [anexos](09_ANEXOS/README.md) guardam material complementar. `src/` e `tests/` recebem a implementação e sua verificação técnica quando houver código. Nem toda ideia exige IA, biomarcadores ou hardware: mantenha apenas as seções pertinentes e registre as escolhas de escopo.

## Como usar

1. Clique em **Use this template** no GitHub e crie um novo repositório para a ideia.
2. Comece pelo [PROJECT.md](PROJECT.md): nomeie o problema, o público, o uso pretendido, a hipótese principal e o estágio atual. Substitua os campos entre `{{chaves}}`.
3. Preencha o [brief](00_VISAO/brief.md) e a [lacuna de evidências](01_EVIDENCIAS/lacuna.md). Separe fatos verificados, interpretação da equipe e hipóteses.
4. Detalhe as frentes necessárias para a ideia. Faça a hipótese corresponder a um método, uma métrica e um critério de aceitação antes de declarar que a solução funciona.
5. Registre mudanças de direção em [DECISIONS.md](DECISIONS.md) e pendências em [STATUS.md](STATUS.md). Marque uma entrega como concluída somente quando houver artefato ou evidência revisada.
6. Use o [guia de contribuição](CONTRIBUTING.md) para trabalhar com colegas e transformar partes do projeto em apresentações, propostas ou candidaturas específicas.

### Formas de aproveitá-lo

- **Explorar uma ideia:** começar pelo problema, alternativas, literatura e incertezas críticas antes de escolher a solução técnica.
- **Organizar pesquisa aplicada:** conectar hipótese, protocolo, fontes de dados, comparadores e validação em documentos rastreáveis.
- **Preparar um portfólio de tecnologia:** mostrar diferencial, estágio de desenvolvimento, evidências existentes, próximos marcos e limites da proposta.
- **Planejar uma colaboração:** explicitar dependências, competências, responsabilidades ainda abertas e entregas que podem ser verificadas.
- **Preparar material para fomento ou transferência:** derivar um resumo e um plano de trabalho dos documentos do projeto, ajustando-os à chamada ou ao interlocutor. O template não substitui regras de editais nem revisão especializada.

## Padrões que orientam o trabalho

- **Rastreabilidade:** cada afirmação relevante deve apontar para fonte, decisão, método ou resultado; referências entram na [matriz](08_REFERENCIAS/matriz.md).
- **Clareza de estágio:** hipótese, plano, protótipo e resultado observado são coisas diferentes. Descreva cada um pelo que de fato existe.
- **Validação proporcional à alegação:** uma demonstração técnica pode provar funcionamento do código, mas não desempenho clínico ou utilidade no cuidado.
- **Segurança e governança:** não inclua no Git dados pessoais ou clínicos individuais, bases restritas, segredos ou credenciais. Use dados sintéticos ou agregados autorizados em exemplos; documente acesso e aprovações antes de usar dados humanos.
- **Revisão por domínio:** afirmações clínicas, éticas, regulatórias e de segurança exigem avaliação adequada ao projeto e ao contexto de uso.

## Sobre a autoria

Este template foi estruturado por [Leonardo Olimpio](https://github.com/leonardoolimpiousp-lang) como uma forma de organizar o desenvolvimento de tecnologias em saúde com rigor científico, decisões explícitas e caminhos verificáveis de execução. Os arquivos são exemplos do método de trabalho; cada projeto criado a partir deles deve construir e documentar suas próprias evidências.
