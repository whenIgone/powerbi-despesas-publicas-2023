# Estados do Brasil e suas Despesas Públicas (2023) — Power BI

Projeto de Data Visualization em **Power BI** com dados abertos de **Execução da Despesa** (Portal da Transparência), com três dashboards: visão geográfica por estado, visão categórica por função (Federal vs Estadual) e visão temporal por órgão.  
Fonte/dicionário de dados: https://portaldatransparencia.gov.br/dicionario-de-dados/execucao-despesa

## Objetivo
Transformar tabelas de despesas públicas em uma visualização interativa para responder:
- Onde estão concentrados valores e operações (visão por UF/Estado)?
- Em que o dinheiro é gasto (funções e subfunções)?
- Como os valores se comportam ao longo do ano e quais órgãos concentram mais despesas?

## Dashboards (o que você encontra)
1. **Estados do Brasil e suas Despesas Públicas (2023)**
   - KPIs de valor (empenhado/liquidado/pago), % pago vs empenhado, distribuição por estados e visão mensal.
2. **Disposição de valores em funções (Federais e Estaduais)**
   - Top 10 funções por valores e participação Federal vs Estadual.
3. **Despesas por Órgão Público ao longo do ano (2023)**
   - Evolução mensal e ranking Top 5 de órgãos superiores, com lista de órgãos subordinados.

## Dados
Arquivo de entrada: `despesaspublicas2023.xlsx` (extraído de dados abertos do Portal da Transparência).  
Campos utilizados incluem tempo (ano-mês), UF/Estado, órgão (superior/subordinado), função/subfunção e valores de execução (R$) como empenhado, liquidado e pago.

> Observação: se você não encontrar o Excel neste repositório, consulte o dicionário e obtenha os dados pela fonte oficial.

## Como executar
1. Baixe o arquivo `.pbix` em `/report`.
2. Abra no **Power BI Desktop**.
3. Se necessário, atualize o caminho da fonte do Excel (Power Query -> Fonte).

## Decisões de design e boas práticas
- Consistência visual: roxo para **Valor Empenhado** e branco para **Valor Pago** (padrão nas páginas).
- Navegação entre dashboards em um único arquivo (.pbix).
- Filtros por estado/mês/órgão para exploração guiada.

## Vídeo demo
- Link do vídeo: https://youtu.be/LH7bciLLftc?si=uBxZZju7xpGfRX96

## Próximos passos
- Publicar versão interativa (quando possível).
- Melhorar visual de mapa (ex.: configurar Azure Maps) e performance.
- Documentar medidas DAX principais e revisar modelagem.

## Autor
Lucas Rodrigues Ferreira (projeto acadêmico em grupo).
