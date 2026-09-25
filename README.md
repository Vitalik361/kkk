# Backtest Logger

Manual backtesting research terminal for SPY Levels + Net Drift + ES Absorption.

## Design
- SPY Levels are manual. You can source them from GEXBOT, QuantData, TradingView, options data, or any other service.
- No live market-data dependency.
- The app records the trader's final setup decision and calculates R/results.
- Browser localStorage is the MVP storage layer.
- Optional Notion sync is included through a server-side API route.

## Run
npm install
npm run dev

Open http://localhost:3000

## Notion
A matching Notion database named BACKTEST TRADES has been created in the connected workspace.

1. Create a Notion integration and share the database with it.
2. Copy .env.example to .env.local.
3. Set NOTION_TOKEN and NOTION_DATABASE_ID.
4. Restart the dev server.

The database schema is already prepared for the logger fields.
