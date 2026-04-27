# Trade System

Each signal generates a structured trade plan.

## Entry
Triggered on confirmed trend flip.

## Stop Loss
Defined using:
- ATR-based buffer
- Recent pivot level (whichever is further)

## Take Profits
Three levels:
- TP1
- TP2
- TP3

Defined using R-multiples of risk.

## Dynamic TP

Targets scale based on:
- Trend Quality Index (TQI)
- Volatility regime

This allows the system to:
- Capture larger moves in strong trends
- Exit earlier in weak conditions
