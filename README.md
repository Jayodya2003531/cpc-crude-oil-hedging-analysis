# cpc-crude-oil-hedging-analysis
Quantitative investigation of CPC’s 2007–2008 oil hedging contracts and design of a 2026–2027 Three-Way Collar hedge using Black-Scholes  and Monte Carlo simulation . 
# CPC Oil Hedging Investigation & Alternative Hedge Design 

An academic quantitative finance and risk-management case study examining the **Ceylon Petroleum Corporation (CPC)** 2007–2008 crude oil hedging program and designing a forward-looking hedging structure for **1 August 2026 – 31 July 2027**.

## Overview
- **Part A — Historical & Structural Diagnosis (2007–2008):** Analyzes WTI price dynamics (Jan 2007 – Dec 2009), structural flaws in CPC's original contracts (such as asymmetric payoff exposure, 2× put multipliers, basis risk, and governance/oversight gaps), and why the sharp price collapse in late 2008 triggered severe mark-to-market losses and legal disputes.
- **Part B — Alternative Hedge Design (Aug 2026 – Jul 2027):** Evaluates hedging structures for a 12-month import exposure (1,000,000 bbl/month) using option pricing (Black-Scholes / Black-76), a **5,000-path Monte Carlo simulation**, 7-point deterministic stress scenarios, and a 30,000-path tail-stress test for a **Guarded Capped Collar**.

## Key Findings & Recommended Structure
- **Recommended Core Hedge:** **Three-Way Collar** — Long Call ($75/bbl), Short Put ($60/bbl), and Long Put ($50/bbl).
- **Risk & Cost Impact (5,000-path Monte Carlo vs. Unhedged):**
  - Reduces average annual import cost by **~$45.08M** (~$3.76/bbl).
  - Lowers effective price standard deviation from **$13.63/bbl** to **$6.14/bbl** while capping upside exposure at **$75/bbl** and bounding extreme downside via the $50 long put.
- **Tail Extension:** Stress-testing a **Guarded Capped Collar** (adding a $130 tail-guard call over 30,000 paths) demonstrates how bounding upper-tail risk reduces worst-case exposure compared to an unguarded short call.

## Methods & Tools
- **Pricing & Simulation:** Black-Scholes / Black-76 option valuation, Monte Carlo simulation (5,000 and 30,000 paths), deterministic scenario analysis, and multi-criteria strategy scoring.
- **Tools:** Microsoft Excel, Python (optional script extensions), Financial/Risk Modeling.

## Team & Context
Completed as part of **FM3015 — Case Study for Finance** (Department of Mathematics, University of Colombo).
- *Group B Contributors:* R.M.M.I.K. Rathnayake, R.H.C.N. Gunarathna, K.V.D.J.C. Karavita, L.A.N.A. Jayasinghe.
