# Template de projeto deeptech em saúde

Modelo reutilizável inspirado na organização documental do VASC-HEMO. Serve para projetos de diagnóstico, dispositivos, software, IA, biotecnologia e pesquisa translacional. Os arquivos são pontos de partida, não afirmações sobre um projeto específico.

## Criar um projeto

1. Clique em **Use this template** no GitHub e crie um repositório para a nova ideia, ou use este diretório como base local.
2. Substitua os campos entre `{{chaves}}` em `PROJECT.md` e nos demais arquivos usados.
3. Registre decisões em `DECISIONS.md`; registre incertezas e dependências em `STATUS.md`.
4. Apague seções não aplicáveis, especialmente IA, biomarcadores ou hardware, após registrar a decisão.
5. Antes de trabalhar com dados de pessoas, documente acesso, base legal, aprovações e ambiente autorizado. Não coloque dados clínicos individuais no Git.

## Mapa

| Local | Pergunta central |
|---|---|
| `00_VISAO/` | Qual problema e proposta de valor? |
| `01_EVIDENCIAS/` | O que sabemos e qual a lacuna? |
| `02_PESQUISA/` | O que será testado e como? |
| `03_DADOS/` | Quais dados existem e podem ser usados? |
| `04_TECNOLOGIA/` | Como construir e reproduzir a solução? |
| `05_VALIDACAO/` | Como medir desempenho, segurança e utilidade? |
| `06_PRODUTO/` | Qual uso pretendido, regulação, PI e negócio? |
| `07_EXECUCAO/` | Quem faz o quê, com quais marcos e riscos? |
| `08_REFERENCIAS/` | Quais fontes sustentam as afirmações? |
| `09_ANEXOS/` | Material complementar e protocolos. |
| `src/`, `tests/` | Código e testes quando houver implementação. |

`PROJECT.md` é o índice e fonte de verdade do projeto. `STATUS.md` reflete apenas trabalho comprovado. Materiais de pitch são derivados da documentação técnica.

## Portões de avanço

- **Ideia → pesquisa:** problema, público, uso pretendido e hipótese definidos.
- **Pesquisa → protótipo:** evidência, viabilidade técnica e acesso a dados ou materiais avaliados.
- **Protótipo → validação:** versão congelada, comparador, métricas e protocolo definidos.
- **Validação → uso real:** resultados revisados, riscos e requisitos éticos/regulatórios tratados conforme o contexto.

Nenhum portão é aprovação clínica ou regulatória automática.
