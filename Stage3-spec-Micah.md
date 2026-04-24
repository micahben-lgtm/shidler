Skip to content
New chat
Agents
Spaces
Spark
Preview
micahben-lgtm
Copilot Free

Create FIN-321 quantitative specification document
Copilot Chat
Create FIN-321 quantitative specification document
scenarios.md
FIN321_AI_Hedging_Project.pptx
You said: Create a fin-321 draft 2–3 page quantitative
Create a fin-321 draft 2–3 page quantitative specification with the information from stage 2 for my excel template Beniamina.Micah-stage2-model.xlsx and format from courses/FIN-321-International-Finance-And-Securities/project-fx-hedging/stage3-spec-assignment.md while using scenario 4 from @adamwstauffer/shidler/files/courses/FIN-321-International-Finance-And-Securities/project-fx-hedging/scenarios.md and taking into consideration @adamwstauffer/shidler/files/courses/FIN-321-International-Finance-And-Securities/project-fx-hedging/FIN321_AI_Hedging_Project.pptx
 

Please include our branding and colors, etc in spec: Found here docs/_branding/design.json
3/3
3/3
Copilot finished thinking

Copilot said: I'll help you create a quantitative specification
I'll help you create a quantitative specification for the FIN-321 FX hedging project. Let me first gather the necessary information from the files you've referenced.Now I'll create a comprehensive, branded Stage 3 Technical Specification for your FX Hedging project using Scenario 4 (U.S. Aerospace Manufacturer). This document will follow the template structure, incorporate UH Mānoa branding, and be formatted for professional readability.

adamwstauffer / shidler / courses / FIN-321-International-Finance-And-Securities / project-fx-hedging / stage3-spec-Micah.md

---
**UNIVERSITY OF HAWAIʻI AT MĀNOA**  
Shidler College of Business | FIN 321: International Finance & Securities

**Prepared by:** Beniamina Micah  
Summary
I've created a comprehensive, UH Mānoa–branded 3-page Stage 3 Technical Specification for your FX Hedging project using Scenario 4 (U.S. Aerospace Manufacturer, $20M EUR receivable). The document includes:

✅ Professional branding — UH Mānoa header, colors (#024731 green), instructor credit
✅ Complete input variables — Spot, forward (1.0935), strikes, premiums, all with named ranges
✅ Detailed calculation flows — Forward, money market, put, and call strategies with step-by-step formulas
✅ Sensitivity analysis plan — ±13.6% spot range, 1% increments, payoff diagram interpretation
✅ Model review section — What worked, what to improve, missing metrics
✅ Clear outputs — Summary tables, sensitivity charts, premium costs, risk metrics
✅ Realistic limitations — Hedge accounting, credit risk, bid–ask spreads, dynamic hedging deferred to Stage 4
✅ Next steps — Direct integration pathway for refined Excel build and AI prompt engineering

You can now copy this content into a markdown file named stage3-spec-Micah.md in your course folder, or I can help you refine any section. The spec is ready to guide both your Stage 2 model improvements and your Stage 4 AI integration work.

give it to me in code for github
Workbench
Press Delete to close the focussed tab.

stage3-spec-Micah.md

"stage3-spec-Micah.md"


338 lines · 17 KB

"stage3-spec-Micah.md" file contents
278
279
280
281
282
283
284
285
286
287
288
289
290
291
292
293
294
295
296
297
298
299
300
301
302
303
304
305
306
307
308
309
310
311
312
313
314
315
316
317
318
319
320
321
322
323
324
325
326
327
328
329
330
331
332
333
334
335
336
337
338

3. **Call option line:**
   - Downside: Falls 1:1 with spot rate below strike, minus premium.
   - Upside: Flat at $21,390,000 (strike minus premium) for S_T > $1.0935.
4. **Unhedged line:** 45° slope upward (no protection, full participation).

**Key takeaway:** The chart visually demonstrates the risk-return tradeoff:
- **Forwards:** Certainty at cost of foregone upside.
- **Put:** Expensive protection ($380K premium) but full upside.
- **Call:** Cheap upside cap but downside exposure.

### **Strategy Comparisons**
- **Put vs. Forward:** Put costs $380K premium but captures upside above ~$1.11; forward foregoes all upside.
- **Put vs. Unhedged:** Put limits downside to $21.49M (vs. $19M unhedged); tradeoff: pay $380K premium.
- **Call vs. Unhedged:** Call caps at $21.39M but costs $480K; worse downside than unhedged below ~$1.08.

---

## 8. Limitations & Next Steps

### **Explicitly Excluded**

| Topic | Why Deferred |
|-------|-------------|
| **Hedge accounting (ASC 815)** | Requires journal entries and P&L timing; deferred to Stage 4 qualitative analysis. |
| **Credit/counterparty risk** | Assumes zero default; in practice, add 5–10 bp for bank/broker credit spread. |
| **Bid–ask spreads & fees** | Ignored; real costs ~10–30 bp reduce net proceeds. |
| **Dynamic hedging** | Model holds hedge to maturity; rolling hedges or intra-period rebalancing excluded. |
| **Dividend yield (FX interest)** | Interest rate differential captured in forward rate; not modeled separately. |
| **Volatility smile / skew** | Black–Scholes assumes flat volatility; real options markets show skew. |
| **Embedded optionality** | No early settlement, optional payment terms, or capped contract provisions. |

### **Next Steps — Stage 4 Integration**

This specification feeds directly into **Stage 4 (Final Recommendations + AI Prompt Engineering)**:

1. **Refined Excel model:** Use this spec to rebuild the model with improved naming, logic, and layouts.
2. **AI prompt:** Provide this document (Section 2–5 especially) to an LLM to:
   - Auto-generate formulas for sensitivity table.
   - Create dynamic charting logic.
   - Suggest alternative hedge structures (collar, seagull, etc.).
3. **Recommendation synthesis:** Combine Stage 3 technical analysis with Stage 4 strategic context (company risk tolerance, cash flow, competitive positioning) to recommend the optimal hedge strategy.

---

## 9. References & Data Sources

- **Spot/Forward rates:** Bloomberg Terminal or Yahoo Finance (record date and time).
- **Interest rates:** 
  - USD: Federal Reserve SOFR/SOFR Board (https://www.sofr.org).
  - EUR: ECB EURIBOR (https://www.ecb.europa.eu/stats/euribor).
- **Option premiums:** Interactive Brokers, CBOE FX options, or Black–Scholes pricing.
- **Instructor guidance:** Adam W. Stauffer, adamstau@hawaii.edu.

---

**END OF SPECIFICATION**

---

*This document was prepared for educational purposes as part of **FIN 321: International Finance & Securities** at the Shidler College of Business, University of Hawaiʻi at Mānoa. All market data and pricing are illustrative; actual execution requires consultation with a financial professional and real-time market quotes.*

Use Control + Shift + m to toggle the tab key moving focus. Alternatively, use esc then tab to move to the next interactive element on the page.
