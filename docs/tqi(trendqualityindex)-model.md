# Trend Quality Index (TQI)

TQI is a normalized score (0 to 1) representing current market quality.

## Components

### 1. Efficiency
Measures directional movement vs total price movement.

### 2. Volatility Regime
Measures whether volatility is expanding or contracting.

### 3. Structure
Measures price position within recent range.

### 4. Momentum Persistence
Measures consistency of directional movement.

## Formula

TQI = weighted average of all four components

Each component is normalized to [0,1].

## Purpose

- High TQI → trending conditions
- Low TQI → choppy conditions

This value drives all adaptive behavior in SATS.
