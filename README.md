# About Quanta Athena

In the institutional landscape, success depends on far more than execution speed — it requires understanding *structure*.  
**Quanta Athena** operates within that structure: it quantifies how implied volatility, strike distance, and time decay shape the probabilistic distribution of future prices.

Developed as the analytical core of the Quanta trading suite, Athena fuses **options-informed analytics**, **statistical modelling**, and **dynamic capital optimisation** into a single adaptive system.  
It continuously evaluates **put-call parity**, **volatility skew**, and **expected move distributions** to locate asymmetrical setups — where risk is quantifiable and the reward profile is statistically justified.

Athena doesn’t chase volatility — it *interprets* it.  
By using real-time option mark data, Black-Scholes probability models, and regime-aware scaling, Athena aligns its trade logic with prevailing volatility states — expanding, contracting, or hedging intelligently as the structure of risk evolves.

---

## 🔍 Core Features

- **Black-Scholes Pricing & ITM Probability**  
  Computes theoretical call/put prices and *N(d₂)* probabilities using live implied volatility, strike, time-to-expiry, and risk-free rate assumptions.

- **Parity-Informed Spot Validation**  
  Derives a synthetic spot price from put-call parity to verify feed accuracy and directional bias, bridging the option and spot markets.

- **Option-Implied Rails**  
  Calculates volatility-based expiry bounds and straddle envelopes, dynamically adjusting order targets to current expected-move distributions.

- **Volatility-Adaptive Engine**  
  Recalibrates order offsets, overlap tolerances, and layer weights based on real-time implied volatility and skew behaviour.

- **Dynamic Capital Optimisation**  
  Allocates exposure in proportion to regime strength, targeting capital efficiency under varying liquidity and volatility conditions.

- **Confluence Scoring Framework**  
  Integrates multi-factor inputs — structural price data, IV trends, skew slope, and time decay — into a unified probabilistic signal.

- **Contextual Risk Management**  
  Modulates trade frequency, exposure, and stop parameters automatically as volatility regimes shift.

- **Data-Driven Execution Layer**  
  Low-latency order engine with adaptive rate-limiting, retry logic, and JSON state persistence for deterministic strategy recovery.

---

## 📊 Included Components

- **Athena Algorithm for Gunbot**  
  Executes Athena’s live strategy logic across supported spot exchanges, incorporating option-implied decision layers.

- **Athena Configuration Profiles**  
  Pre-built template optimised for low-, medium-, and high-volatility environments, ensuring stable execution across regimes.

---

## ⚙️ Platform Compatibility

**Quanta Athena** is licensed exclusively for deployment on the **Gunbot** automated trading platform.

---

## 🧠 Technical Overview

| Domain | Description |
|:--|:--|
| **Analytical Core** | Black-Scholes engine (price, ITM %, expected move), volatility-skew mapping, put-call parity validation |
| **Execution Logic** | Regime-aware buy/sell order generator with offset scaling, layer weighting, and timer-based gating |
| **Risk Control** | BEP-aware capital throttling, soft capital ceilings, adaptive frequency modulation |
| **Persistence** | JSON state storage via proxy handler; maintains runtime continuity across cycles |
| **Refresh Logic** | Dynamic API polling cadence (1–60 min) based on IV delta intensity |
| **Visual Output** | Custom chart rails (IV expiry, straddle bounds, BS marks, parity spot) and detailed side-bar telemetry (ROC, ECR, IV state) |

---

### “Fortuna Eruditis Favet”  
*Fortune favours the informed.*

**Quanta Athena — Market-Neutral Intelligence for Volatile Markets**
