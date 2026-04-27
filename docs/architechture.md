# System Architecture

SATS follows a modular pipeline:

1. Market State Measurement
   - Compute TQI from 4 factors

2. Volatility Adjustment
   - Compute ATR and efficiency-weighted ATR

3. Band Construction
   - Apply adaptive multipliers
   - Smooth values (EMA)

4. Signal Engine
   - Price-based flip
   - Character-based flip

5. Trade Engine
   - Entry, SL, TP generation

6. Tracking Engine
   - Monitor TP/SL hits
   - Compute realized R

7. Analytics Layer
   - Rolling stats
   - Regime-based edge tracking
