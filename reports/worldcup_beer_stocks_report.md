# World Cup Beer Stocks: A Market Sentiment Analysis

## 1. Overview

This project examines whether the results of the final knockout rounds 
of the FIFA World Cup have a measurable impact on the stock prices of 
publicly traded beer companies. More specifically, it asks whether the 
presence or elimination of specific nations in the quarter finals, semi 
finals and final drives meaningful stock price movements — and whether 
those movements follow a predictable enough pattern to inform investment 
decisions as the tournament progresses.

The analysis covers five World Cup tournaments from 2010 to 2026, 
tracking ten publicly traded beer companies across six geographic markets. 
By building a beer alignment scoring framework — which measures how 
strongly associated each remaining nation is with beer consumption culture 
— the project attempts to quantify what the market intuitively senses: 
that not all teams are equal in their impact on beer demand.

This project was built and published during the 2026 World Cup, with the 
semi finals still to be played. The four remaining teams — France, Spain, 
England and Argentina — are among the most beer-aligned nations in the 
tournament's history, making the next four days one of the most 
consequential periods for beer stocks in recent World Cup history.

## 2. Central Question

The central question of this analysis is whether public equity markets 
correctly anticipate the consumption implications of World Cup results — 
and whether the elimination of high beer-consumption nations produces 
measurable, consistent negative stock reactions in the companies most 
exposed to those markets.

A secondary question emerged during the analysis: do markets price in 
the World Cup effect before it happens — buying beer stocks in 
anticipation of a tournament — and then sell once matches actually take 
place? This "buy the rumour, sell the news" dynamic, if present, would 
suggest that the stock movements are driven by market sentiment rather 
than genuine consumption changes, and that the window for trading on 
World Cup results may be narrower than conventional wisdom suggests.

## 3. Data and Methodology

Ten publicly traded beer companies were selected to represent the major 
geographic beer markets most likely to be affected by World Cup results:

| Ticker | Company | Market |
|---|---|---|
| BUD | AB InBev | Global (Official World Cup Sponsor) |
| ABEV | Ambev | Brazil and Latin America |
| TAP | Molson Coors | USA, Canada and England |
| STZ | Constellation Brands | Mexico |
| HEINY | Heineken | Europe |
| CABGY | Carlsberg | Denmark and Eastern Europe |
| ASBRF | Asahi | Japan |
| KNBWY | Kirin | Japan |
| SAM | Boston Beer | USA |
| CCU | Cervecerias Unidas | Chile and South America |

Five tournaments were analysed — 2010 through 2026 — covering the period 
for which reliable price data exists for all ten companies. Not all beer 
stocks have trading history beyond 2010, making that the natural starting 
point. The 2026 tournament is included as a live dataset, with the semi 
finals still to be played at the time of publication.

The analytical framework was built in two layers. The first was a 
**beer alignment score** — a metric designed to quantify how strongly 
each remaining nation is associated with beer consumption culture, on a 
scale of 0 to 10. This was constructed manually based on per capita beer 
consumption and cultural association with beer. High scorers include 
England (9), Belgium (9), Germany (10) and Netherlands (9). Low scorers 
include Morocco (2), Saudi Arabia (1) and Qatar (0). The score was 
applied to every match in the quarter finals, semi finals and final 
across all five tournaments, allowing comparison of beer cultural 
alignment across different tournament outcomes.

The second layer was a series of quantitative analyses run against 
historical stock price data:

- **Price summary** — establishing baseline price characteristics for 
  each company across the full 2010–2026 period
- **World Cup vs non-World Cup windows** — comparing average stock prices 
  on match days against the rest of the year
- **Pre-tournament returns** — testing the "buy the rumour, sell the 
  news" hypothesis by measuring stock performance in the 90 days before 
  each tournament began
- **Elimination impact by nation** — calculating the average 5-day stock 
  return after each beer-relevant nation was eliminated, to identify 
  which country's exit hurt stocks most
- **Finals ranked by beer alignment** — identifying which historical 
  finals were most and least beer-aligned, and what that implies for 
  the 2026 outcome
- **Prediction model** — applying the historical elimination impact data 
  to all four possible 2026 final combinations to generate directional 
  stock predictions

## 4. Key Findings

**Finding 1: Beer alignment varies dramatically within Europe — 
country matters more than continent.**
The analysis confirms that generalising by continent is misleading. 
Within Europe alone, beer alignment scores range from England (9/10) 
and Belgium (9/10) at the top to France (6/10) and Switzerland (6/10) 
at the lower end. Germany scores a perfect 10/10. This means a 
"European" final can be anywhere from highly beer-aligned to moderately 
aligned depending on which specific nations are involved. The practical 
implication is that country-level analysis is essential — continent-level 
analysis produces noise rather than signal.

**Finding 2: England's elimination is the single most damaging event 
for beer stocks.**
Across all five tournaments, when England was eliminated from the 
quarter finals or semi finals, the beer stocks most exposed to the 
UK market fell an average of 4.69% in the following five trading days. 
This is more than four times larger than the impact of Argentina's 
elimination (-1.13%) and dwarfs the effect of any other nation studied. 
TAP (Molson Coors) is the primary stock to watch when England's 
tournament fate is decided.

**Finding 3: The market buys the rumour and sells the news.**
The 2014 tournament produced the clearest evidence of pre-tournament 
speculation — beer stocks rose an average of 15.1% in the 90 days 
before kickoff, then fell 4.5% in the 20 days after matches during 
the knockout rounds. 2018 showed a smaller version of the same pattern 
(+2.4% pre, -2.5% during). This suggests investors anticipate the 
consumption boost of a beer-aligned tournament and price it in advance 
— then sell once the matches actually happen, rather than waiting for 
revenue to materialise in company financials.

**Finding 4: Qatar 2022 is the natural experiment that proves 
the contrarian case.**
The 2022 tournament was an outlier in every respect — a dry host 
country, Morocco's unexpected semi final run pushing the beer 
alignment score to its lowest of any tournament studied (6.2/10), 
and a December scheduling that broke the summer pattern. Yet it 
produced the only positive average post-match return in the study 
(+0.49%). This supports the hypothesis that when a tournament is 
widely expected to be bad for beer stocks, contrarian investors 
buy the dip — and the lack of pre-tournament speculation means 
there is no sell-off to follow.

**Finding 5: The best case scenario for beer stocks is 
England vs Argentina in the final.**
This finding is counterintuitive. Most observers would assume a 
French or Spanish final would benefit European beer stocks most. 
But the data tells a different story — when France or Belgium are 
eliminated, beer stocks historically tick upward slightly, meaning 
their exit is not the damaging event it might appear. England's 
presence in the final keeps TAP supported while France and Spain 
exiting the semi finals generates small positive reactions via 
HEINY and CABGY. The net result of an England vs Argentina final 
with England winning is the most positive total tournament impact 
at +0.25% — the only scenario in the entire model that produces 
a positive combined return across semi finals and final.

## 5. Limitations and Alternative Explanations

**Small sample size.**
Five tournaments — four completed — is a very small dataset from 
which to draw statistical conclusions. Each tournament-level finding 
is based on four data points, meaning a single unusual tournament 
like Qatar 2022 can heavily influence the averages. A more robust 
analysis would require at least ten tournaments, which would mean 
extending the data back to the 1980s — a period for which reliable 
stock price data for most of these companies does not exist. The 
findings presented here should be treated as directional signals 
rather than statistically significant results.

**The beer alignment score is a subjective framework.**
The beer alignment score was constructed manually based on cultural 
association and per capita consumption estimates — it is not a 
statistically derived metric. Different analysts applying the same 
framework might assign meaningfully different scores to the same 
nations. The entire prediction model rests on this subjective 
foundation, which limits its precision. A more rigorous version 
would derive the scores empirically from consumption data correlated 
against historical stock returns.

**Macroeconomic confounding factors.**
The analysis does not control for broader market movements, interest 
rates, commodity prices, or sector-specific events that may have 
influenced beer stock prices during tournament windows. The post-
financial-crisis context of 2010, for example, likely explains why 
that tournament deviated most sharply from the expected pattern. 
Without controlling for these factors, it is impossible to isolate 
the World Cup effect cleanly from the market environment it occurred in.

**Currency effects.**
Several stocks in the study trade primarily outside the United States — 
HEINY, CABGY, NVO and ASBRF in particular. USD-denominated price 
movements for these stocks may partly reflect currency fluctuations 
rather than genuine beer consumption signals, introducing noise into 
the analysis.

**Tournament path not tracked.**
This analysis focused exclusively on the quarter finals, semi finals 
and final — the last three rounds. It did not track the full 
tournament path of specific nations from the group stage onwards, 
which means early-stage momentum effects, gradual stock build-up 
as a team progresses, and the psychological impact of a team's 
journey are all excluded. A complete analysis would track stock 
reactions from the first group stage match through to elimination.

**2026 data is incomplete.**
The semi finals and final of the 2026 tournament had not been played 
at the time of publication. The 2026 predictions are forward-looking 
applications of historical patterns and should be treated as 
hypotheses to be tested rather than confirmed findings.

## 6. Conclusions and Broader Implications

This analysis set out to answer a deceptively simple question: does 
it matter, for beer stock investors, which teams make it to the final 
rounds of the World Cup? The answer, based on five tournaments of 
historical data, is yes — but not in the way most people would intuitively 
expect.

The market does not wait for beer revenues to appear in quarterly 
filings before repricing stocks. It acts on anticipation, sometimes 
months before a tournament begins, and then corrects once the event 
is actually underway. The "buy the rumour, sell the news" pattern 
identified in 2014 and 2018 suggests that the window for trading on 
World Cup sentiment is narrow — and that by the time the quarter finals 
are being played, much of the movement has already happened.

When it does move during the tournament, it moves asymmetrically. 
England's elimination is catastrophically negative for TAP at -4.69%, 
while France's elimination is actually mildly positive. This asymmetry 
is the most actionable finding in the study — not all eliminations are 
created equal, and the conventional wisdom that "more beer-drinking 
nations in the tournament is always better for stocks" is an 
oversimplification the data does not support.

For the 2026 tournament specifically, the model points to England vs 
Argentina as the best case final for beer stocks — a counterintuitive 
conclusion that follows directly from the data rather than from 
conventional market narrative. With those semi finals still to be 
played at the time of publication, this project has the unusual 
distinction of being a live prediction model rather than a purely 
historical study. Whether the predictions hold will itself be a finding 
worth documenting.

**Broader implication:** The framework developed here — beer alignment 
scoring, elimination impact mapping, pre-tournament sentiment tracking — 
is transferable to other major sporting events. The UEFA European 
Championship, the Copa América, the Rugby World Cup and the Cricket 
World Cup all have their own beverage, hospitality and consumer staples 
exposure stories waiting to be mapped. The methodology is the 
contribution; the World Cup is just the first application.

---
*Analysis by Nicole Otero — Data Analytics Portfolio Project, 2026*  
*Data sourced from Yahoo Finance via yfinance and public FIFA records. 
For research and educational purposes only — not investment advice.*
