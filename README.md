# Sociologia das Prisões: dados e análise da população carcerária brasileira

Repositório de pesquisa sobre o sistema penitenciário brasileiro, construído a partir dos levantamentos oficiais do SISDEPEN/SENAPPEN. Reúne dados brutos, scripts de tratamento, visualizações, fichamentos de leitura, linha do tempo histórica, análise crítica de políticas penais e um mapa de debates teóricos.

## Objetivos

Este repositório sustenta o trabalho desenvolvido na especialização em Gestão de Política Penal (UFSCar), reunindo dados empíricos sobre a população carcerária brasileira como evidência de apoio às análises produzidas ao longo do curso — em diálogo com discussões sobre seletividade penal, desigualdade racial e o Plano Pena Justa.

[EDITAR: se um trabalho específico da especialização for a peça final (título e pergunta de pesquisa), inclua aqui para amarrar o repositório a esse texto.]

## Como navegar

| Seção | O que contém |
|---|---|
| [`linha-do-tempo/`](./linha-do-tempo/historia-das-prisoes.md) | Linha do tempo da história das prisões — eixo internacional (do suplício à prisão moderna) e eixo brasileiro (colônia ao SENAPPEN). |
| [`analise-critica/`](./analise-critica/politicas-penais-brasileiras.md) | Avaliação crítica de políticas penais brasileiras (Lei de Drogas, RDD, ADPF 347, Pacote Anticrime), testando coerência entre discurso, mecanismo e dado empírico. |
| [`dados/`](./dados/README.md) | Banco de indicadores do sistema prisional em CSV/JSON, com fonte e data para cada valor. |
| [`debates-teoricos/`](./debates-teoricos/README.md) | Fichas de autores clássicos e contemporâneos (Foucault, Goffman, Sykes, Clemmer, Kauffman, Wacquant, Baratta, Malaguti Batista, Gilmore, Quijano, Mbembe) com conceito central, aplicação e limites de cada um. |
| [`fichamentos/`](./fichamentos/README.md) | Resumos, análises críticas, mapas conceituais e fichamentos ABNT de textos processados (aguardando primeiros PDFs). |
| [`data/`, `scripts/`, `docs/`](#estrutura-do-repositório) | Dados brutos, scripts de tratamento (Python/Plotly) e figuras exportadas — ver seção de metodologia abaixo. |
| [`CONTRIBUTING.md`](./CONTRIBUTING.md) | Como contribuir com dados, fichamentos, fichas teóricas ou revisões. |

## Fontes dos dados

Os dados utilizados neste repositório têm origem no **SISDEPEN** (Sistema de Informações do Departamento Penitenciário Nacional), plataforma atualmente operada pela **SENAPPEN** (Secretaria Nacional de Políticas Penais, que sucedeu o antigo DEPEN), por meio dos Levantamentos de Informações Penitenciárias publicados semestralmente.

- Fonte oficial: <https://www.gov.br/senappen/pt-br/servicos/sisdepen>
- Levantamento(s) utilizado(s): [EDITAR — ex. "1º semestre de 2025"]
- Data de extração: [EDITAR — data em que os dados foram baixados]

> **Nota metodológica:** os números do SISDEPEN/SENAPPEN são autodeclarados pelas unidades federativas e sujeitos a defasagem e inconsistência de atualização entre estados.

## Estrutura do repositório

```
sociologia-das-prisoes/
├── data/
│   ├── raw/                # extrações originais, sem alteração
│   └── processed/          # dados tratados, gerados pelos scripts abaixo
├── scripts/                 # tratamento e visualização (Python/Plotly)
├── docs/                    # figuras exportadas (uso futuro: GitHub Pages)
├── dados/                    # indicadores consolidados em CSV/JSON, com fonte e data
│   ├── indicadores-sisdepen.csv
│   ├── indicadores-sisdepen.json
│   └── README.md
├── linha-do-tempo/
│   └── historia-das-prisoes.md
├── analise-critica/
│   └── politicas-penais-brasileiras.md
├── debates-teoricos/         # uma ficha de autor por arquivo
│   └── README.md
├── fichamentos/               # resumo + análise + mapa conceitual + fichamento por texto
│   ├── _template/
│   └── README.md
├── CONTRIBUTING.md
├── LICENSE           # licença do código (MIT)
└── README.md
```

## Metodologia

[EDITAR — descreva em poucas linhas o fluxo: como os dados brutos foram obtidos, que tratamento cada script aplica, e que critérios de seleção/recorte foram usados (ex.: só São Paulo, só determinado período, só determinada variável).]

O banco de indicadores em [`dados/indicadores-sisdepen.csv`](./dados/indicadores-sisdepen.csv) segue uma regra própria: cada linha carrega sua fonte, URL e data de publicação, e valores ainda não localizados em fonte comparável ficam marcados como `PENDENTE` em vez de estimados — ver [`dados/README.md`](./dados/README.md) para o dicionário de dados completo e as pendências conhecidas.

## Limitações

- Dados autodeclarados pelas unidades federativas, sem auditoria externa centralizada.
- Mudanças de metodologia e de sistema (transição SISDEPEN → SENAPPEN) podem afetar a comparabilidade entre séries históricas — ver exemplo concreto dessa divergência entre 2025-S1 e 2025-S2 em [`dados/README.md`](./dados/README.md).
- A análise crítica e a linha do tempo são documentos de trabalho, com lacunas explicitamente sinalizadas (ver seção 6 de [`analise-critica/politicas-penais-brasileiras.md`](./analise-critica/politicas-penais-brasileiras.md)), não levantamentos exaustivos.
- [EDITAR — qualquer limitação específica do recorte adotado: unidade de análise, variáveis ausentes, período coberto.]

## Como contribuir

Ver [`CONTRIBUTING.md`](./CONTRIBUTING.md) para como adicionar dados, fichamentos, fichas de debates teóricos ou revisões e correções.

## Licença

- **Código** (pasta `scripts/`): licenciado sob [MIT](LICENSE).
- **Dados e textos originais** (`dados/`, `linha-do-tempo/`, `analise-critica/`, `debates-teoricos/`, `fichamentos/`): disponibilizados sob [Creative Commons Atribuição 4.0 Internacional (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/deed.pt-br) — uso e redistribuição livres, desde que citada a fonte (SISDEPEN/SENAPPEN, quando aplicável) e este repositório.

## Como citar

José Erivaldo Ferreira Silva. *Sociologia das Prisões: dados e análise da população carcerária brasileira*. GitHub, 2026.
ORCID: 0009-0004-1589-9888 · Lattes: 6829697063257893

## Autor

Policial Penal (SAP-SP), instrutor na Escola de Administração Penitenciária (EAP), pós-graduando em Gestão de Política Penal (UFSCar). Pesquisa na interseção entre sociologia institucional, criminologia crítica e experiência profissional.
