# Banco de dados de indicadores do sistema prisional

`indicadores-sisdepen.csv` / `indicadores-sisdepen.json` — mesmo conteúdo em dois formatos, um indicador por linha.

## Dicionário de dados

| Campo | Descrição |
|---|---|
| `indicador` | Nome do indicador em snake_case (ex.: `populacao_carceraria_total`) |
| `valor` | Valor numérico bruto, sem formatação (sem separador de milhar) |
| `unidade` | `pessoas`, `vagas`, `percentual`, `atendimentos` |
| `periodo_referencia` | Semestre/ano a que o dado se refere (ex.: `2025-S2`), não a data em que foi publicado |
| `abrangencia` | `Brasil` ou unidade da federação |
| `fonte` | Órgão/publicação de origem |
| `url_fonte` | Link para a fonte primária |
| `data_publicacao` | Data em que o dado foi tornado público |
| `observacoes` | Ressalvas metodológicas, divergências entre séries, ou motivo de o campo estar vazio (`PENDENTE`) |

## Regras de uso deste banco

1. **Nunca misturar séries sem checar a metodologia.** Este banco já registra um caso concreto: a população total de `2025-S1` (941.752) inclui prisão domiciliar; a de `2025-S2` (727.301) parece referir-se apenas a pessoas em cela física. Comparar as duas diretamente como "queda de população" seria um erro de leitura — está sinalizado no campo `observacoes` da linha correspondente.
2. **Todo indicador tem fonte rastreável.** Se você adicionar um indicador, ele precisa de `url_fonte` e `data_publicacao` — sem isso, um dado não entra no CSV/JSON, só na lista de pendências abaixo.
3. **Vazio é `PENDENTE`, não zero.** Um valor vazio significa que o indicador é relevante mas ainda não foi localizado em fonte comparável — nunca preencher com zero ou estimativa não sinalizada como tal.

## Pendências conhecidas (oportunidades de contribuição)

- Distribuição por cor/raça consolidada em nível nacional para o período mais recente (2025-S2) — o relatório SENAPPEN indica que o dado existe nas páginas 85-86 do PDF original, mas não foi extraído nesta rodada.
- Distribuição por faixa etária (2025-S2) — mesma situação.
- Distribuição por nível de escolaridade (2025-S2).
- Taxa de reincidência por unidade da federação — não localizada em fonte oficial consolidada; necessária para testar o argumento da seção 5 de [`/analise-critica/politicas-penais-brasileiras.md`](../analise-critica/politicas-penais-brasileiras.md).
- Série histórica (2015–2025) de taxa de ocupação nacional, para permitir avaliar o efeito da ADPF 347 (2015) ao longo do tempo, não apenas em dois pontos.

Ver [`CONTRIBUTING.md`](../CONTRIBUTING.md) para como propor a inclusão de um indicador.
