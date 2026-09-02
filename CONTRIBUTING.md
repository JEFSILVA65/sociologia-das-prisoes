# Como contribuir

Este repositório reúne pesquisa sobre a população carcerária brasileira e sociologia das prisões, mantido por [José Erivaldo Ferreira Silva (JEFSILVA65)](https://github.com/JEFSILVA65) — Policial Penal e pós-graduando em Gestão de Políticas Penais (UFSCar). Contribuições são bem-vindas nas quatro frentes abaixo. O padrão de rigor é o mesmo em todas: nenhuma contribuição entra sem fonte rastreável (para dados) ou sem a seção de tensão/limite (para conteúdo teórico) — ver os protocolos já aplicados em [`/analise-critica/`](./analise-critica/politicas-penais-brasileiras.md) e [`/debates-teoricos/`](./debates-teoricos/README.md).

## Formas de contribuir

### 1. Dados

Adicionar ou corrigir um indicador em [`/dados/indicadores-sisdepen.csv`](./dados/indicadores-sisdepen.csv) (e seu equivalente `.json`). Toda linha nova precisa preencher `fonte`, `url_fonte` e `data_publicacao` — sem isso, a contribuição não é aceita como dado, apenas registrada como pendência. Ver as regras completas em [`/dados/README.md`](./dados/README.md).

### 2. Fichamentos

Processar um novo texto (livro, capítulo, artigo) nos quatro formatos descritos em [`/fichamentos/README.md`](./fichamentos/README.md): resumo, análise crítica, mapa conceitual e fichamento ABNT. **Não subir o PDF original** — apenas os quatro documentos derivados, que são produção autoral sobre o texto.

### 3. Debates teóricos

Criar ou revisar uma ficha de autor em [`/debates-teoricos/`](./debates-teoricos/README.md). Toda ficha precisa das quatro seções: conceito central, o que explica bem, onde falha ou exige mediação teórica, e diálogo com outros autores da pasta. Uma ficha que só resume o autor sem a seção de limite não está completa.

### 4. Revisões e correções

Correção de datas na [linha do tempo](./linha-do-tempo/historia-das-prisoes.md), reconciliação de séries de dados divergentes, ou identificação de saltos argumentativos na [análise crítica](./analise-critica/politicas-penais-brasileiras.md) — inclusive discordâncias de interpretação, desde que fundamentadas.

## Como submeter

1. Abra uma *issue* descrevendo a contribuição antes de um PR extenso, para alinhar escopo.
2. Para mudanças pontuais (uma linha de dado, uma correção de data), um Pull Request direto é suficiente.
3. Cite sempre a fonte primária — para dados, um link oficial (SISDEPEN/SENAPPEN, IBGE, STF, Diário Oficial); para teoria, a edição usada.
4. Textos com direitos autorais de terceiros: apenas fichamentos e citações breves com página, nunca o texto integral.

## Licença

Código sob licença MIT (ver [`LICENSE`](./LICENSE)). Dados e textos originais deste repositório sob [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/deed.pt_br), salvo indicação em contrário.
