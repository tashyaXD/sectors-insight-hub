# Sectors Intelligence Hub

Design and build a high-fidelity web application called Sectors Terminal, a Market Intelligence platform for the Indonesian stock market.

The product is inspired by the information density and analytical capabilities of professional financial terminals such as Bloomberg Terminal, but it must NOT visually copy Bloomberg. The goal is to create an original, modern, highly professional financial intelligence interface that feels analytical, premium, data-driven, and distinctive.

1. PRODUCT PURPOSE

Sectors Terminal consumes market, company fundamental, sector, and news data from the Sectors REST API / MCP and transforms raw data into derived insights.

This is NOT a simple stock dashboard.

The core product value is:

Raw Sectors Data → Data Processing → Custom Analysis / Scoring → Derived Insight → Decision Support

The interface must make this analytical transformation obvious to users.

Do NOT design the product as a generic dashboard that only displays raw API data.

The application must emphasize:

custom financial scores

rankings

anomaly detection

peer comparison

financial risk analysis

sentiment and catalyst analysis

rule-based screening

Automated trading and trade execution must NOT exist anywhere in the application.

2. MAIN NAVIGATION

Create a professional desktop-first web application with a persistent left sidebar navigation.

Main navigation:

Market Overview

Sector Intelligence

Company Terminal

News Intelligence

Decision Screener

Secondary navigation/settings:

Search

Watchlist

Export Insights

Methodology

Settings

The interface should feel like an analytical workstation rather than a conventional marketing website.

3. VISUAL DIRECTION

Use a sophisticated neutral financial color system.

Primary visual direction:

Deep graphite / charcoal

Warm off-white

Soft gray

Muted slate

Very restrained teal/cyan accent

Green and red ONLY for financial positive/negative states

Avoid:

bright blue SaaS dashboards

excessive gradients

neon cyberpunk aesthetics

excessive glassmorphism

excessive rounded cards

generic purple AI aesthetics

overly colorful charts

excessive shadows

childish or playful UI

The interface should feel:

professional

intelligent

calm

analytical

premium

slightly unconventional

information-dense

easy to scan

Use mostly square or subtly rounded components rather than heavily rounded cards.

Suggested visual palette:

Background:

#111315

#17191C

#202327

Surface:

#24282C

#2B3035

Primary text:

#F2F1EC

Secondary text:

#A7ADB3

Borders:

#383D42

Accent:

muted teal / cyan such as #58B8B0

Positive:

restrained green

Negative:

restrained red

Warning:

muted amber

The accent color should be used sparingly for active navigation, important analytical highlights, selected states, and key insights.

Do not make every component colorful.

4. TYPOGRAPHY

Use a clean modern sans-serif typeface such as Inter, Geist, IBM Plex Sans, or a similar professional UI font.

Use:

compact typography

strong hierarchy

tabular-looking numbers

clear numerical alignment

smaller metadata labels

bold values for important metrics

Financial numbers should be highly scannable.

Use uppercase or small-caps styling sparingly for section labels and metadata.

5. INFORMATION DENSITY

The UI should intentionally support high information density.

However, avoid visual clutter.

Use:

compact tables

analytical panels

score badges

mini charts

sparklines

heatmaps

comparison matrices

structured data rows

expandable analysis sections

tooltips

Avoid making every piece of information a large card.

Large empty spaces should be minimized on analytical pages.

6. PAGE 1 — MARKET OVERVIEW

Create a dashboard that immediately answers:

"What is happening in the Indonesian market right now?"

Header

Include:

page title: Market Overview

current market status

last updated timestamp

global search

date/time context

Market Snapshot

Create a compact horizontal metrics section showing:

IHSG

daily change

percentage change

market status

number of advancing stocks

number of declining stocks

Do not make these overly large.

IHSG Chart

Create a large but compact area chart/line chart showing IHSG movement.

Include selectable time periods:

1D

1W

1M

3M

1Y

Sector Heatmap

Create a large interactive heatmap of Indonesian stock sectors.

Each sector should show:

sector name

performance percentage

optional market capitalization indicator

The heatmap should visually communicate relative sector performance.

Sector Health Index

Create a prominent analytical section titled:

Sector Health Index

Show ranked sectors with:

rank

sector

SHI score 0–100

growth

margin stability

debt condition

trend

health status

Example:

Technology — 84 — Strong Financials — 76 — Healthy Consumer — 63 — Moderate

SHI is a CUSTOM DERIVED SCORE.

Add an information tooltip explaining that the score is calculated from weighted indicators such as:

growth

margin stability

debt ratio

The tooltip should NOT simply say "from API".

Market Anomaly Monitor

Create a panel showing automatically detected market anomalies.

Each anomaly should include:

company

sector

detected metric

company value

sector average

deviation

anomaly severity

Example:

BBXX Banking P/E 28.7x Sector average 15.2x +88.1% deviation Valuation divergence detected

Make it visually distinct from normal market data.

7. PAGE 2 — SECTOR INTELLIGENCE

This page is the deep research environment for individual sectors.

Header:

Sector Intelligence

sector selector

search

date range

Sector Summary

Show:

selected sector

sector performance

SHI

sector trend

number of companies

Sector Performance

Show:

sector performance chart

comparison against IHSG

historical trend

Fundamental Comparison

Create a comparison table/chart for:

revenue growth

profitability

margin

debt ratio

valuation

other relevant available metrics

Sector Health Breakdown

Create a visual breakdown of SHI.

For example:

SHI 84

Growth: 88 Margin Stability: 81 Debt Condition: 79

Use horizontal bars or compact analytical indicators.

Company Universe

Create a dense sortable table containing companies in the selected sector.

Columns:

ticker

company

price

change

market cap

growth

profitability

debt

valuation

company health

anomaly status

Sector Divergence Detector

Create an analytical panel titled:

Sector Divergence

This detects companies whose metrics significantly deviate from their sector baseline.

For each detected divergence show:

Company Metric Company Value Sector Average Deviation Interpretation

Example:

Company A P/E 28.7x Sector average 15.2x +88.1% Valuation Divergence

This must visually communicate that the system has generated an insight rather than merely displayed API data.

8. PAGE 3 — COMPANY TERMINAL

Create a professional company comparison workspace.

The user should be able to select between 2–5 companies.

Example: BBCA BBRI BMRI

Company Search

Include fast search/autocomplete for:

ticker

company name

sector

Peer Comparison Matrix

Create a dense comparison table.

Rows:

revenue growth

profit margin

ROE

debt ratio

valuation

dividend

market performance

other available fundamental indicators

Columns: selected companies.

Use subtle visual highlighting to make differences easy to scan.

Head-to-Head Dominance Score

Create a prominent analytical component:

Dominance Score

Score each selected company based on a CUSTOM weighted matrix.

Possible factors:

growth

profitability

ROE

debt

valuation

market performance

Show:

final score

factor contribution

comparison

Example:

Company A — 82 Company B — 74 Company C — 68

Do NOT describe this as a buy/sell recommendation.

It is a comparative analytical score.

Include a tooltip:

"Dominance Score is a custom weighted comparison across selected fundamental and market indicators."

Financial Safety & Distress

Create a separate analytical section:

Financial Safety

Show:

score 0–100

risk category

leverage

liquidity

profitability

financial stability

Allow the system to use a modified financial scoring methodology such as Altman Z-Score / Piotroski F-Score or a custom methodology depending on available Sectors data.

Include a "How is this calculated?" interaction.

9. PAGE 4 — NEWS INTELLIGENCE

This page should NOT look like a normal news website.

It should look like an analytical news terminal.

News Feed

Display news from Sectors data with:

timestamp

headline

company

sector

source

sentiment

catalyst type

impact level

Sentiment Classification

Automatically classify news into:

Positive Neutral Negative

Use subtle indicators, not huge colorful labels.

Catalyst Classification

Classify news into categories such as:

earnings

dividend

corporate action

expansion

acquisition

regulatory

management

other relevant catalysts

Impact Mapping

Show how each news item relates to: News → Company → Sector → Potential Impact

Example:

Company A Positive Catalyst Expansion Technology Sector Impact: Medium

News Filters

Allow instant filtering by:

company

sector

sentiment

catalyst

impact

date

10. PAGE 5 — DECISION SCREENER

Create a powerful analytical screening interface.

The purpose is to help users filter companies based on multiple factors.

Do NOT include automated trading or buy/sell execution.

Screening Factors

Allow users to configure filters based on:

SHI

growth

profitability

debt

valuation

dividend

financial safety

anomaly status

Multi-Factor Decision Matrix

Create a rule-based classification system.

Example classifications:

Undervalued Quality

relatively attractive valuation

strong profitability

strong financial safety

Growth at Reasonable Price

strong growth

valuation within configured threshold

High Dividend Trap Alert

high dividend yield

weaker fundamental/financial safety indicators

These are ANALYTICAL CLASSIFICATIONS generated by predefined rules, not trading recommendations.

Screening Result

Use a dense table:

Ticker Company Sector SHI Growth Financial Safety Valuation Dividend Classification

Allow sorting and filtering.

11. EXPLAINABILITY / METHODOLOGY

Create a dedicated Methodology area.

Every custom score must be explainable.

For each score show:

What is being measured?

Which indicators are used?

Weight of each indicator

Normalization method

Score calculation

Interpretation

This is especially important for:

Sector Health Index

Dominance Score

Financial Safety Score

Anomaly Detection

Sentiment Classification

Decision Matrix

The UI should make these explanations accessible through:

tooltips

"How calculated?" buttons

expandable methodology panels

12. SEARCH EXPERIENCE

Create a global search command interface.

Users should be able to search:

companies

ticker symbols

sectors

news

The search should feel fast and professional.

Consider a keyboard-friendly command/search interface inspired by financial terminals and developer tools.

For example:

Search: BBCA

Results: Company Sector Recent News Sector Position Financial Safety Anomalies

13. EXPORT INSIGHTS

Add an Export action to relevant analytical pages.

Users should be able to export:

peer comparison

sector research

screening results

anomaly reports

decision matrix

Possible formats:

PDF

copy as text

The exported content should preserve:

title

timestamp

selected companies/sectors

important metrics

derived scores

methodology summary

14. INTERACTION DESIGN

Use smooth but restrained interactions.

Important interactions:

hover tooltips

expandable rows

sortable tables

instant filters

dropdown selectors

chart hover states

heatmap hover states

modal/detail drawer for deeper analysis

Avoid excessive animations.

The application should feel fast and analytical.

Use subtle transitions around 150–250ms.

15. RESPONSIVE DESIGN

Primary target: Desktop / laptop.

The product is an analytical terminal, so desktop should receive the most attention.

Still make it usable on tablet and smaller screens.

On mobile:

prioritize key metrics

convert wide tables into horizontal scrolling

stack analytical panels

preserve navigation usability

Do NOT sacrifice analytical readability just to make everything fit on mobile.

16. COMPONENT SYSTEM

Create a reusable design system containing:

Sidebar

Top navigation

Metric strip

Analytical card

Compact data table

Score badge

Health indicator

Anomaly badge

Sentiment badge

Heatmap cell

Chart container

Tooltip

Filter dropdown

Search command palette

Comparison matrix

Expandable methodology panel

Export button

Detail drawer

Keep components visually consistent across all pages.

17. IMPORTANT PRODUCT CONSTRAINTS

The website MUST:

consume Sectors API / MCP data

generate custom derived insights

clearly distinguish raw data from calculated insights

explain custom scoring methodologies

support market, sector, company, and news analysis

provide decision-support screening

The website MUST NOT:

execute trades

automatically buy or sell securities

function as an automated trading bot

pretend that custom scores are official market ratings

overwhelm users with decorative UI

18. DESIGN CHARACTER

The final interface should feel like:

"A modern Indonesian market intelligence workstation."

Not:

generic fintech dashboard

generic SaaS admin panel

crypto trading interface

Bloomberg clone

AI chatbot dashboard

The visual identity should be original.

Use asymmetrical but balanced layouts where appropriate.

Mix:

dense analytical tables

thin dividers

compact cards

large typography for only the most important metrics

subtle accent lines

charts

heatmaps

information panels

Create visual hierarchy through spacing, typography, borders, and contrast rather than excessive colors.

The result should feel sophisticated enough for financial research while remaining understandable to a university-level user.

19. MOCK DATA

For the initial UI/UX prototype, use realistic Indonesian stock-market mock data.

Use Indonesian companies/sectors as placeholder examples, but clearly structure the application so these values can later be replaced by Sectors API data.

Prioritize realistic-looking financial values and relationships between metrics.

Do not hardcode the analytical methodology into the visual appearance; keep the score calculation logic modular so it can later be connected to the actual backend.

20. FINAL UI GOAL

When opening the application, the user should immediately understand:

What is happening in the Indonesian market?

Which sectors are showing notable conditions?

Which companies are behaving differently from their peers?

How do selected companies compare fundamentally?

What financial risks or strengths are detected?

What important catalysts are appearing in the news?

Which companies match a selected analytical screening rule?

The product should communicate:

DATA → ANALYSIS → INSIGHT

at every major interaction.

Build the UI/UX as a polished, high-fidelity prototype rather than a generic dashboard template.

This project was built with [Lovable](https://lovable.dev).

**Live app**: https://sectors-insight-hub.lovable.app

## Build with Lovable

Continue developing this project in the [Lovable editor](https://lovable.dev/projects/fec535e6-7fc0-427a-a4cf-db816aa25d95).

- **Ship faster**: describe what you want to build and Lovable handles the code.
- **Stay in sync**: every change made in Lovable is committed straight to this repository.
- **Full ownership**: this code is yours. Push to `main` on GitHub and your changes sync back into Lovable, ready for your next prompt.

## Development

Prefer working locally? You need Node.js and npm — [install with nvm](https://github.com/nvm-sh/nvm#installing-and-updating).

```sh
git clone <this-repository-url>
cd <repository-name>
npm i
npm run dev
```
