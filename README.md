# SATS-Trend-System
Self-Aware Trend System (SATS): Adaptive SuperTrend with real-time Trend Quality Index (TQI) and regime-aware behavior.
SATS — Self-Aware Trend System
Adaptive SuperTrend with real-time market awareness and built-in performance tracking.
SATS is a trend-following system that adjusts itself based on current market conditions using a proprietary Trend Quality Index (TQI). Instead of fixed parameters, it dynamically adapts to whether the market is trending or choppy.

# Key Features
## Trend Quality Index (TQI)
Measures market quality every bar using four factors:
* Efficiency (directional movement vs noise)
* Volatility regime
* Market structure
* Momentum persistence
Outputs a score from 0 to 1 representing trend strength.

## Adaptive SuperTrend
* Bands tighten in strong trends to lock profits
* Bands widen in choppy markets to reduce whipsaws
* Uses non-linear scaling for realistic adaptation
## Asymmetric Bands
* Active band tightens to protect profit
* Passive band widens to avoid premature exits
Character-Flip Detection
* Detects trend failure before price breaks bands
* Uses TQI collapse with a minimum trend age filter

# Trade System
Each signal generates:
* Entry (on confirmed flip)
* Stop Loss (pivot + ATR buffer)
* Take Profits (TP1, TP2, TP3 using R-multiples)
Dynamic Take-Profit 
* Targets scale based on:
    * Trend quality (TQI)
    * Volatility
* Expands in strong conditions, contracts in weak ones
* Fixed mode still available

Performance Tracking
Tracks all signals in real time:
* Win rate
* Average R
* Drawdown (rolling and all-time)
* Win/loss streaks
Regime-Based Analysis
* Trades classified into 9 market regimes
* Shows performance per regime
* Helps identify where the system has an edge

# How It Works
1. Compute TQI from four factors
2. Adjust ATR to effective volatility
3. Apply adaptive multiplier
4. Smooth values to prevent instability
5. Build SuperTrend bands
6. Detect flips (price or character-based)
7. Generate trade plan
8. Track outcomes and update stats

# How to Use
1. Add the indicator (Auto preset recommended)
2. Follow the trend line:
    * Green = bullish
    * Red = bearish
    * Bright = strong trend, faded = weak
3. Enter on signal labels (BUY/SELL)
4. Use plotted Entry, SL, and TP levels
5. Monitor performance in the dashboard

# Tuning Guide
* Too many false signals → Increase Quality Influence
* Signals too late → Reduce band width
* Choppy market → Enable Character Flip, increase minimum age
* Strong trends → Increase asymmetry

# Important Notes
* No repainting (signals confirmed on bar close)
* TQI is descriptive, not predictive
* Performance stats are forward-tracked, not backtested
* Auto-calibration is experimental (off by default)
* This is a decision-support tool, not an automated trading system


# Alerts
* BUY / SELL signals
* Includes price, TQI, SL, TP levels, and TP mode
* Supports webhook and text formats

# Summary
SATS replaces static indicators with a system that measures market conditions, adapts its behavior, and tracks its own performance in real time.

