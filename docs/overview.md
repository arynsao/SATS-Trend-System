# SATS Overview

SATS (Self-Aware Trend System) is an adaptive trend-following system built on a modified SuperTrend framework.

The system introduces a real-time market quality metric (TQI) and uses it to dynamically adjust band width, signal logic, and trade management.

## Core Idea

Traditional indicators are static.

SATS measures:
- Whether the market is trending or noisy
- How strong that trend is
- Whether the trend is degrading

Then adjusts its behavior accordingly.

## Components

- Trend Quality Index (TQI)
- Adaptive SuperTrend Engine
- Character-Flip Detection
- R-based Trade System
- Performance Tracking Engine
