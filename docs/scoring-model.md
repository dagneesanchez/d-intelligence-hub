# D-Intelligence Hub — Relevance Scoring Model

## 1. Purpose

The relevance scoring model determines how important each news item is for
the objectives of D-Intelligence Hub.

The initial score ranges from 0 to 100.

The score is designed to prioritize information rather than simply measure
whether a news item is interesting.

---

## 2. Scoring Dimensions

Each news item is evaluated across six dimensions.

| Dimension | Weight |
|---|---:|
| Economic relevance | 20% |
| Investment relevance | 25% |
| Payments relevance | 20% |
| Geographic relevance | 15% |
| Potential future impact | 10% |
| Source quality | 10% |
| Total | 100% |

---

## 3. Economic Relevance

Measures the potential importance of the news for the economy or financial
environment.

Examples of high relevance:

- Major central bank decisions
- Significant inflation changes
- Major fiscal policy changes
- Important economic indicators
- Major financial crises

Examples of low relevance:

- Minor economic commentary
- Repetitive market commentary
- News with limited economic consequences

Score range:

0–100

---

## 4. Investment Relevance

Measures how relevant the news could be for an investment portfolio.

Examples:

- Direct impact on an asset
- Important company-specific developments
- Sector-wide changes
- Interest rate changes
- Currency movements
- Commodity price shocks

Score range:

0–100

---

## 5. Payments Relevance

Measures how relevant the information is to payments, fintech and related
business models.

Examples:

- Payment networks
- Payment processors
- Digital wallets
- Instant payments
- Open banking
- Acquiring
- Issuing
- Fraud prevention
- Payment orchestration
- Fintech regulation

Score range:

0–100

---

## 6. Geographic Relevance

Measures the importance of the geographic context.

Higher relevance should generally be assigned to:

1. Argentina
2. Latin America
3. United States
4. Europe
5. Global developments

The geographic relevance should depend on the specific topic rather than
using geography as an absolute ranking.

Score range:

0–100

---

## 7. Potential Future Impact

Measures whether the news could become more important over time.

High scores may be assigned to:

- Early regulatory signals
- Emerging technologies
- Structural economic changes
- New business models
- Early-stage industry trends
- Changes that could create future opportunities

Score range:

0–100

---

## 8. Source Quality

Measures the reliability and usefulness of the information source.

Higher scores should generally be assigned to:

- Official institutions
- Central banks
- Government agencies
- Regulatory bodies
- Established financial institutions
- High-quality financial news organizations

Lower scores should be assigned when:

- The source is unclear
- The information is highly speculative
- The article lacks supporting evidence

Source quality should not automatically determine the overall relevance of
a story.

Score range:

0–100

---

## 9. Initial Score Calculation

The weighted score can be represented as:

```text
Score =
(Economic Relevance × 0.20)
+
(Investment Relevance × 0.25)
+
(Payments Relevance × 0.20)
+
(Geographic Relevance × 0.15)
+
(Future Impact × 0.10)
+
(Source Quality × 0.10)
The final score is normalized to a range from 0 to 100.
10. Relevance Levels
Score	Level
80–100	Critical
60–79	High
40–59	Medium
20–39	Low
0–19	Ignore


11. Explainability
Every relevance score should include reasons explaining why the news item
received its score.
Example:
Score: 87

Reasons:
- Major central bank decision
- Direct impact on interest rates
- Relevant to financial markets
- High-quality source
- Potential portfolio implications
The system should avoid producing unexplained scores.
12. Future Improvements
The initial scoring model is rule-based.
Future versions may incorporate:
- Historical user feedback
- Topic-specific scoring
- Asset-level relevance
- Sector-level relevance
- Machine learning
- LLM-assisted classification
- Personal relevance adjustments
The scoring model should evolve based on observed results and user feedback.
