# Compras-peças · MCPO Irrigação

Painel de métricas de compras e estoque de peças (Faturamento, Curva ABC, Inventário, Giro, Sortimento, Zero Vendas).

- Publicado em: https://mcpoirrigacao.github.io/compras-estoque/
- Login com a conta Microsoft da MAQCAMPO (mesmo registro de app do Azure dos demais apps MCPO).
- Os dados **não** ficam neste repositório. Eles ficam na pasta do SharePoint MCPOIRRIGACAO:
  - `compras_pecas_dados.json` — base completa do painel
  - `compras_pecas_acesso.json` — lista de administradores e usuários comuns
- Aba **Parâmetros** (só administradores): cadastro de usuários, situação da pasta e importação/exportação da base.
- **Atualizar dados** (só administradores): envia o `Métrica Mensal.xlsx` e/ou o `Estoque Histórico.xlsx`; o painel recalcula e grava a base no SharePoint.

## Configuração no Azure (uma vez)

Cadastrar `https://mcpoirrigacao.github.io/compras-estoque/` como Redirect URI do tipo **Single-page application (SPA)** no registro de app `a02d9ccd-9650-4855-99ce-3ad5ec98c381`.
