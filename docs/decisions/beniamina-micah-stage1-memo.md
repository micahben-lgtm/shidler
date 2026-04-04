# U.S. Aerospace Manufacturer – FX Receivable Hedging Proposal

**Created by:** Micah Beniamina  
**Updated by:** Micah Beniamina  
**Date Created:** April 3, 2026  
**Date Updated:** April 3, 2026  
**Version:** 1.0  
**LLM Used:** None

---

## Executive Summary (≤150 words)

Our firm faces a material EUR 18.5 million receivable due in one year from a European aerospace component supply contract. At current spot rates (~1.09 USD/EUR), this exposure represents approximately $20 million in uncertain USD proceeds. Currency depreciation could reduce our revenue by 2–5% if the euro weakens. This memo outlines our FX exposure and proposes three hedging strategies—forward contracts, protective puts, and zero-cost collars—to protect shareholder value. We recommend proceeding to Stage 2, where we will model each strategy's payoff across realistic market scenarios and quantify the cost-benefit tradeoff for management's decision.

---

## Background & Objectives

**The Exposure:** Our company has contracted to receive EUR 18.5 million from a major European client in exactly one year (April 3, 2027). At today's spot rate of approximately 1.0935 USD/EUR, this represents roughly $20.2 million in expected USD revenue. However, FX volatility creates material risk: a 3% euro depreciation would reduce our proceeds to $19.6 million, representing a $600,000 loss. A 5% depreciation would cost us roughly $1 million.

**Why It Matters:** Our operating margins in the aerospace supply industry average 4–6%. A significant FX loss could materially impact annual earnings and shareholder returns. Our CFO and Board are therefore evaluating whether a hedging strategy is prudent.

**Objective:** Evaluate three hedging approaches and recommend a strategy that balances protection with cost, enabling us to lock in economics while maintaining strategic flexibility for favorable rate movements.

---

## Methods

We will analyze three hedging families:

1. **Forward Contract (One-Year Forward)** – Lock in the forward rate of 1.0935 today for settlement in one year. Pros: Certain payoff, zero upfront cost, simple execution. Cons: No upside participation, fully obligatory (may underperform if euro strengthens).

2. **Protective Put (EUR Put Option)** – Buy a EUR put option at strike ≈1.0935 with premium $0.019 per contract. Pros: Downside protection with upside capture if euro appreciates. Cons: Premium cost (~$0.019/EUR = $351,500 total), reduces net proceeds.

3. **Zero-Cost Collar (Buy Put + Sell Call)** – Buy a protective put at 1.0935 and simultaneously sell a EUR call at a higher strike (e.g., 1.12). Pros: Downside protection, minimal or zero upfront cost, defined risk/reward. Cons: Caps upside gains above the call strike.

**Data & Tools:** We will use current market quotes (forward rates, option premiums), build a sensitivity model in Excel, and compute P&L outcomes under a range of EUR/USD scenarios at maturity.

**Next Steps:**
- **Stage 2:** Build a working Excel model comparing realized USD proceeds under each hedge strategy across market scenarios.
- **Stage 3:** Document the model structure, assumptions, and formula logic in a technical specification.
- **Stage 4:** Analyze model output, formulate a final recommendation, and present the case to the CFO and Board.

---

## Limitations & Next Steps

**Limitations:** 
- Our analysis assumes a 1-year horizon and does not account for interim cash flows or early unwind scenarios.
- Option premiums and forward rates are placeholders pending real-time market data retrieval.
- We do not yet model accounting treatment (ASC 815) or tax implications, which may influence final recommendation.

**Immediate Next Steps:**
1. Source current EURUSD spot and forward rates (as of market close today, April 3, 2026).
2. Retrieve current EUR option premiums from Bloomberg or broker quotes.
3. Source USD and EUR interest rate curves to validate forward rate and discount factors.
4. Build Stage 2 Excel model.

---

## References

- Scenario 4, FIN-321 Project Briefing, Adam W. Stauffer, 2026.
- CME FX Futures and Options; Bloomberg Terminal data (to be sourced in Stage 2).
- Class Notes: International Parity Conditions and Hedging Strategies, FIN-321, Spring 2026.