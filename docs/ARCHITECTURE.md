# ARCHITECTURE — VORTEX HUNTER

## Purpose
Market and opportunity scanner — hunts for vortex patterns (momentum, convergence) in financial markets, trends, or business opportunities.

## System Overview
```
[Market Data]  --> [Pattern Scanner] --> [Vortex Detector]
[Alert Engine] --> [Dashboard]       --> [Action Queue]
```

## Components
- **Market Data**: Real-time price, volume, options flow feeds
- **Pattern Scanner**: Technical indicator computation (momentum, volume surge)
- **Vortex Detector**: Multi-signal confluence scoring
- **Alert Engine**: Real-time notifications on detected vortexes
- **Action Queue**: Prioritized opportunity list with expiry

## Data Flow
Raw Data → Scan → Score → Alert → Review → Act

## Integration Points
- SUPERSTONK-TRADER (execution)
- TESLACALLS2026 (options-specific feed)
- Matrix Monitor (live opportunity display)

## Key Decisions
- Detection over prediction — find patterns, not crystal ball
- All alerts include confidence score and time window
