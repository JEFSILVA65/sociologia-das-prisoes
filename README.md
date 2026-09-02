# Sociologia das Prisões: dados e análise da população carcerária brasileira

Repositório de pesquisa sobre o sistema penitenciário brasileiro, construído a partir
dos levantamentos oficiais do SISDEPEN/SENAPPEN. Reúne dados brutos, scripts de
tratamento e visualizações.

## Objetivos

Este repositório sustenta o trabalho desenvolvido na especialização em Gestão de
Política Penal (UFSCar), reunindo dados empíricos sobre a população carcerária
brasileira como evidência de apoio às análises produzidas ao longo do curso — em
diálogo com discussões sobre seletividade penal, desigualdade racial e o Plano Pena
Justa.

[EDITAR: se um trabalho específico da especialização for a peça final (título e
pergunta de pesquisa), inclua aqui para amarrar o repositório a esse texto.]

## Fontes dos dados

Os dados utilizados neste repositório têm origem no **SISDEPEN** (Sistema de
Informações do Departamento Penitenciário Nacional), plataforma atualmente operada
pela **SENAPPEN** (Secretaria Nacional de Políticas Penais, que sucedeu o antigo
DEPEN), por meio dos Levantamentos de Informações Penitenciárias publicados
semestralmente.

- Fonte oficial: <https://www.gov.br/senappen/pt-br/servicos/sisdepen>
- Levantamento(s) utilizado(s): [EDITAR — ex. "1º semestre de 2025"]
- Data de extração: [EDITAR — data em que os dados foram baixados]

> **Nota metodológica:** os números do SISDEPEN/SENAPPEN são autodeclarados pelas
> unidades federativas e sujeitos a defasagem e inconsistência de atualização entre
> estados. Comparações entre levantamentos de períodos diferentes devem controlar
> explicitamente a data de corte antes de sustentar qualquer inferência de tendência.

## Estrutura do repositório

```
sociologia-das-prisoes/
├── data/
│   ├── raw/          # extrações originais, sem alteração
│   └── processed/    # dados tratados, gerados pelos scripts abaixo
├── scripts/          # tratamento e visualização (Python/Plotly)
├── docs/             # figuras exportadas (uso futuro: GitHub Pages)
├── LICENSE           # licença do código (MIT)
└── README.md
```

## Metodologia

[EDITAR — descreva em poucas linhas o fluxo: como os dados brutos foram obtidos, que
tratamento cada script aplica, e que critérios de seleção/recorte foram usados (ex.:
só São Paulo, só determinado período, só determinada variável).]

## Limitações

- Dados autodeclarados pelas unidades federativas, sem auditoria externa
  centralizada.
- Mudanças de metodologia e de sistema (transição SISDEPEN → SENAPPEN) podem afetar
  a comparabilidade entre séries históricas.
- [EDITAR — qualquer limitação específica do recorte adotado: unidade de análise,
  variáveis ausentes, período coberto.]

## Licença

- **Código** (pasta `scripts/`): licenciado sob [MIT](LICENSE).
- **Dados** (pasta `data/`): disponibilizados sob [Creative Commons Atribuição 4.0
  Internacional (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/deed.pt-br) —
  uso e redistribuição livres, desde que citada a fonte (SISDEPEN/SENAPPEN) e este
  repositório.

## Como citar

José Erivaldo Ferreira Silva. *Sociologia das Prisões: dados e análise da população
carcerária brasileira*. GitHub, 2026.
ORCID: 0009-0004-1589-9888 · Lattes: 6829697063257893

## Autor

Policial Penal (SAP-SP), instrutor na Escola de Administração Penitenciária (EAP),
pós-graduando em Gestão de Política Penal (UFSCar). Pesquisa na interseção entre
sociologia institucional, criminologia crítica e experiência profissional.
