# About Quanta Athena

In the institutional landscape, success depends on more than execution speed; it requires understanding *structure*.  
**Quanta Athena** operates within that structure. It quantifies how implied volatility, strike distance, and time decay shape the probabilistic distribution of future prices.

Developed as the analytical core of the Quanta trading suite, Athena combines **options-informed analytics**, **statistical modelling**, and **dynamic capital optimisation** into a single adaptive system.  
It continuously evaluates **put call parity**, **volatility skew**, and **expected move distributions** to locate asymmetrical setups where risk is measurable and reward potential is statistically justified.

Athena does not chase volatility; it *interprets* it.  
By using real-time option mark data, Black-Scholes probability models, and regime-aware scaling, Athena aligns its trade logic with prevailing volatility states, expanding or contracting intelligently as the structure of risk evolves.

---

## 🔍 Core Features

- **Black-Scholes Pricing and ITM Probability**  
  Computes theoretical call and put prices and *N(d2)* probabilities using live implied volatility, strike, time to expiry and the current risk-free rate.

- **Parity-Informed Spot Validation**  
  Derives a synthetic spot price from put call parity to verify feed accuracy and directional bias, linking the option and spot markets.

- **Option-Implied Rails**  
  Calculates volatility-based expiry bounds and straddle envelopes, dynamically adjusting order targets to the current expected move distribution.

- **Volatility-Adaptive Engine**  
  Recalibrates order offsets, overlap tolerances, and layer weights based on real-time implied volatility and skew behaviour.

- **Dynamic Capital Optimisation**  
  Allocates exposure in proportion to regime strength, maintaining capital efficiency across changing liquidity and volatility conditions.

- **Confluence Scoring Framework**  
  Integrates multiple analytical factors such as price structure, IV trends, skew slope and time decay into a unified probabilistic signal.

- **Contextual Risk Management**  
  Modulates trade frequency, exposure and stop parameters automatically as volatility regimes shift.

- **Data-Driven Execution Layer**  
  Low-latency order engine with adaptive rate limiting, retry logic and JSON state persistence for deterministic strategy recovery.

---

## 📊 Included Components

- **Athena Algorithm for Gunbot**  
  Executes Athena’s live strategy logic across supported spot exchanges, incorporating option-informed decision processes.

- **Athena Configuration Profiles**  
  Pre-built templates optimised for low, medium and high volatility environments to ensure stable execution across regimes.

---

## ⚙️ Platform Compatibility

**Quanta Athena** is licensed exclusively for deployment on the **Gunbot** automated trading platform.

---

## 🧠 Technical Overview

| Domain | Description |
|:--|:--|
| **Analytical Core** | Black-Scholes engine (price, ITM %, expected move), volatility skew mapping, put call parity validation |
| **Execution Logic** | Regime-aware buy and sell order generation with offset scaling, layer weighting and timer-based gating |
| **Risk Control** | Break-even aware capital throttling, capital ceilings and adaptive frequency modulation |
| **Persistence** | JSON state storage via proxy handler to maintain runtime continuity across sessions |
| **Refresh Logic** | Dynamic API polling cadence (1–60 minutes) based on IV delta intensity |
| **Visual Output** | Custom chart rails (IV expiry, straddle bounds, BS marks, parity spot) and sidebar telemetry (ROC, ECR, IV state) |

---

### *Fortuna Eruditis Favet*  
*Fortune favours the informed.*

**Quanta Athena: Market Neutral Intelligence for Volatile Markets**
