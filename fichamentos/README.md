# Fichamentos

Esta pasta recebe, para cada PDF processado, quatro arquivos derivados — nunca o PDF original (ver nota de direitos autorais abaixo):

```
fichamentos/
  <slug-do-texto>/
    resumo.md
    analise-critica.md
    mapa-conceitual.md
    fichamento.md
```

Um `<slug-do-texto>` por obra (ex.: `foucault-vigiar-e-punir/`), para manter os quatro arquivos de um mesmo texto juntos e permitir referência cruzada entre eles.

## O que vai em cada arquivo

**`resumo.md`** — síntese objetiva do conteúdo (argumento central, estrutura do texto, principais evidências mobilizadas pelo autor). Não avalia, apenas reconstrói o que o texto diz.

**`analise-critica.md`** — aplica o protocolo de avaliação deste repositório: coerência lógica (saltos argumentativos, premissas implícitas), consistência teórica (uso correto ou ornamental dos conceitos, lacunas de interlocução), consistência empírica (dados vs. inferência interpretativa, generalizações frágeis) e estrutura acadêmica (coerência entre problema, método, análise e conclusão). Ver o protocolo completo aplicado em [`/analise-critica/politicas-penais-brasileiras.md`](../analise-critica/politicas-penais-brasileiras.md) como modelo de padrão esperado.

**`mapa-conceitual.md`** — representação estruturada (lista hierárquica ou diagrama Mermaid) das relações entre os conceitos centrais do texto e sua conexão com os autores já fichados em [`/debates-teoricos/`](../debates-teoricos/).

**`fichamento.md`** — fichamento no formato acadêmico brasileiro tradicional: referência completa em ABNT (NBR 6023), citações-chave com página, e comentário do leitor separado da citação literal.

Modelos prontos (vazios, com a estrutura esperada) estão em [`_template/`](./_template/).

## Nota sobre direitos autorais

Este repositório é público. **Não versionar os PDFs originais** dos textos estudados — apenas os quatro arquivos derivados acima, que são produção autoral do usuário sobre o texto (resumo, análise, mapa, fichamento), não reprodução da obra. Citações diretas no `fichamento.md` devem ser breves e sempre com indicação de página, conforme uso acadêmico legítimo.

## Como adicionar um novo texto

1. Anexar o PDF na conversa com o assistente (ou colar o texto), para que os quatro documentos sejam gerados.
2. Criar a subpasta `fichamentos/<slug-do-texto>/` a partir de [`_template/`](./_template/).
3. Preencher os quatro arquivos.
4. Adicionar uma linha à tabela abaixo.
5. Se o autor ainda não tem ficha em [`/debates-teoricos/`](../debates-teoricos/), avaliar se vale a pena criar uma.

## Índice de textos fichados

| Texto | Autor | Fichado em | Pasta |
|---|---|---|---|
| _(nenhum ainda — aguardando PDFs)_ | | | |
