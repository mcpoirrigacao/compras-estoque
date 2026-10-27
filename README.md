# Compras-peças · MCPO Irrigação

Painel de métricas de compras e estoque de peças (Faturamento, Curva ABC, Inventário, Giro, Sortimento, Zero Vendas e Compras).

- Publicado em: https://mcpoirrigacao.github.io/compras-estoque/
- Login com a conta Microsoft da MAQCAMPO (mesmo registro de app do Azure dos demais apps MCPO).
- Os dados **não** ficam neste repositório. O painel lê as planilhas da pasta `Compras-estoque` do SharePoint MCPOIRRIGACAO a cada acesso e recalcula tudo no navegador:
  - `Métrica Mensal.xlsx` — Faturamento, Curva ABC, CMV do Giro, Sortimento e Zero Vendas
  - `Estoque Histórico.xlsx` — Giro e evolução do estoque varejo
  - `Inventário_de_Peças.xlsx` — Inventário, saldos da Curva ABC/Sortimento e Zero Vendas
  - `Armazém.xlsx` — nomes dos armazéns (opcional)
  - `DADOS_BI_COMPRAS.csv` — aba **Compras** (pedidos de compra: KPIs, gráficos e detalhamento)
  - `HITORICO_PC.xlsx` — aba **Compras**, coluna "Histórico da Compra"
  - `Filiais.csv` — aba **Compras**, nomes das filiais (Código;Filial)
- O único arquivo gravado pelo painel na pasta é `compras_pecas_parametros.json` (usuários admin/comum e nomes das planilhas).
- Aba **Parâmetros** (só administradores): usuários, situação das planilhas e nomes dos arquivos.
- **Atualizar dados**: lê de novo as planilhas da pasta. O painel também confere sozinho a cada 2 minutos.

## Configuração no Azure (uma vez)

Cadastrar `https://mcpoirrigacao.github.io/compras-estoque/` como Redirect URI do tipo **Single-page application (SPA)** no registro de app `a02d9ccd-9650-4855-99ce-3ad5ec98c381`.
