# World Cup Beer Stocks: A Market Sentiment Analysis

## Overview
An equity research case study examining whether beer stock prices move 
in response to which nations remain in the FIFA World Cup tournament — 
built and published live during the 2026 World Cup with the semi finals 
still to be played at time of publication.

## Central Question
Do beer stock prices correlate with the cultural beer-drinking alignment 
of nations remaining in the World Cup quarter finals, semi finals and 
finals — and does the market correctly anticipate consumption changes 
based on who is still playing?

## Key Findings
- **England's elimination** is the single most damaging event for beer 
  stocks — TAP drops an average of 4.69% in the 5 days following
- **Buy the rumour, sell the news** — beer stocks rose 15.1% before 
  the 2014 tournament then fell 4.5% during it
- **Qatar 2022** was the natural experiment — lowest beer alignment 
  score yet produced the only positive post-match returns (+0.49%)
- **Best case for 2026** — England vs Argentina final with England 
  winning produces the highest combined tournament impact (+0.25%)
- **Country beats continent** — beer alignment varies dramatically 
  within Europe; generalising by region produces noise not signal

## Tournaments Analysed
| Year | Host | Winner |
|---|---|---|
| 2010 | South Africa | Spain |
| 2014 | Brazil | Germany |
| 2018 | Russia | France |
| 2022 | Qatar | Argentina |
| 2026 | USA/Canada/Mexico | TBD (Live) |

## Beer Stocks Tracked
| Ticker | Company | Key Markets |
|---|---|---|
| BUD | AB InBev | Global (Official World Cup Sponsor) |
| ABEV | Ambev | Brazil, Latin America |
| TAP | Molson Coors | USA, Canada, England |
| STZ | Constellation Brands | Mexico (Corona, Modelo) |
| HEINY | Heineken | Netherlands, Europe |
| CABGY | Carlsberg | Denmark, Eastern Europe |
| ASBRF | Asahi | Japan |
| KNBWY | Kirin | Japan |
| SAM | Boston Beer | USA |
| CCU | Cervecerias Unidas | Chile, South America |

## Beer Alignment Score
A custom scoring framework (0-10) measuring each nation's association 
with beer consumption culture. Key scores:

| Nation | Score | Nation | Score |
|---|---|---|---|
| Germany | 10/10 | France | 6/10 |
| England | 9/10 | Argentina | 7/10 |
| Belgium | 9/10 | Morocco | 2/10 |
| Netherlands | 9/10 | Qatar | 0/10 |

## 2026 Prediction Model
With France, Spain, England and Argentina in the semi finals:

| Scenario | Total Impact | Key Stock |
|---|---|---|
| Worst: France vs Spain final | -5.32% | TAP, ABEV |
| Mid: Any final with ARG out in SF | -3.31% to -4.94% | TAP |
| Best: England wins the final | +0.25% | HEINY, CABGY |

## Tools & Methods
- **Python / pandas** — data collection and analysis via yfinance
- **SQL / SQLite** — data structuring and querying
- **Matplotlib** — visualisation
- **Jupyter Notebooks** — analysis environment

## Project Structure

│
├── data/
│   ├── raw/          # Stock prices and World Cup match data
│   └── processed/    # Cleaned outputs and SQL results
├── notebooks/        # Jupyter notebooks
├── sql/              # Standalone SQL query files
├── visualizations/   # Charts and decision tree
├── reports/          # Final written analysis
└── README.md

## Visualisations
- **Beer alignment by tournament** — comparing beer cultural score 
  across all five World Cups
- **Buy the rumour, sell the news** — pre vs post tournament returns
- **Elimination impact chart** — which nation's exit hurts stocks most
- **Decision tree** — all possible semi final and final outcomes 
  with predicted stock impacts

## Status
✅ Complete — built live during the 2026 World Cup

## Author
Nicole Otero — Data Analytics Portfolio Project, 2026
