# Sectors Terminal implementation plan

## Goal
Build a polished desktop-first Indonesian market intelligence workstation that turns realistic mock market data into clearly labeled derived analysis. The first release will be a high-fidelity interactive prototype, structured so a future Sectors API/MCP adapter can replace the mock provider without changing the screens.

## Experience and navigation
- Create a persistent graphite sidebar with Market Overview, Sector Intelligence, Company Terminal, News Intelligence, and Decision Screener, plus Search, Watchlist, Export Insights, Methodology, and Settings.
- Add a compact top bar with market status, Jakarta time context, last-updated state, global command search, and page actions.
- Use separate shareable routes for every major area, with route-specific metadata.
- Provide a collapsible mobile/tablet navigation while preserving horizontal scrolling for dense tables.

## Design system
- Establish the specified charcoal, warm off-white, muted slate, restrained teal, positive green, negative red, and warning amber as semantic tokens.
- Use IBM Plex Sans with tabular numerals, compact type, thin dividers, square/subtly rounded surfaces, restrained shadows, and 150–250ms transitions.
- Build reusable terminal primitives: shell, panel, metric strip, table, score/health/anomaly/sentiment indicators, heatmap cell, chart frame, tooltip, filters, search palette, comparison matrix, methodology disclosure, export menu, and detail drawer.

## Data and analytical layer
- Create a typed mock data provider with realistic Indonesian indexes, sectors, listed companies, fundamentals, market history, anomalies, and news.
- Keep derived calculations separate from display data: Sector Health Index, Dominance Score, Financial Safety, anomaly deviation, sentiment/catalyst tags, and screening classifications.
- Label source observations versus calculated insights throughout the interface and expose weights/formulas in contextual explanations.

## Screens
- **Market Overview:** compact IDX snapshot, interactive IHSG range chart, sector heatmap, ranked Sector Health Index, and anomaly monitor.
- **Sector Intelligence:** sector/date selectors, sector-versus-IHSG chart, fundamental comparison, SHI breakdown, sortable company universe, and divergence analysis.
- **Company Terminal:** 2–5 company selector, comparison matrix, weighted Dominance Score, factor contributions, and Financial Safety analysis.
- **News Intelligence:** dense terminal feed with filters, subtle sentiment/catalyst/impact states, and company-to-sector impact mapping.
- **Decision Screener:** configurable multi-factor filters, predefined analytical classifications, and sortable result table.
- **Methodology:** explain measurement, indicators, weights, normalization, formula, and interpretation for each custom model.
- **Watchlist and Settings:** focused supporting screens matching the terminal shell; export actions will support copy-to-clipboard and print/PDF workflow.

## Interaction and validation
- Implement command search, table sorting, time-range selection, sector/company selectors, instant news/screener filters, expandable methodology, detail drawers, and export actions.
- Verify the live interface at desktop and mobile widths, including search, navigation, filters, comparison selection, table overflow, and visible chart/heatmap states.
- Confirm every content route has unique title, description, Open Graph, and Twitter metadata.

## Scope boundary
- No trade execution, order entry, buy/sell recommendations, or automated trading.
- This iteration uses realistic mock data only; live Sectors API/MCP connectivity remains an adapter step because no connector credentials or endpoint contract were provided.
