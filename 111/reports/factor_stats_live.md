# Factor Evaluation

## Overview

- **audit_events_total**: `17122`
- **directional_decisions_total**: `12868`
- **unique_markets**: `146`
- **decisions_with_trade_result**: `366`
- **decisions_without_trade_result**: `12502`
- **traded_markets**: `47`
- **winning_trades**: `22`
- **losing_trades**: `25`
- **total_pnl**: `-17.4033`
- **avg_pnl**: `-0.3703`
- **win_rate**: `0.4681`

## D1-D8 Factors

| factor | name | weight | active | neutral | missing | active rate | avg abs contribution | win rate active | avg pnl active |
|---|---|---:|---:|---:|---:|---:|---:|---:|---:|
| D1 | Price vs Price-to-Beat | - | 12462 | 256 | 150 | 96.8% | 1.8351 | 38.9% | -0.6305 |
| D2 | Time-adjusted ATR Distance | - | 12462 | 256 | 150 | 96.8% | 1.3661 | 38.9% | -0.6305 |
| D3 | Multi-horizon Return Slope | - | 12125 | 593 | 150 | 94.2% | 0.6625 | 35.3% | -0.7823 |
| D4 | Window VWAP / TWAP Position | - | 10029 | 2689 | 150 | 77.9% | 0.7089 | 41.2% | -0.5735 |
| D5 | Path Structure | - | 8503 | 4215 | 150 | 66.1% | 0.4513 | 50.0% | -0.1625 |
| D6 | Mean Reversion Risk | - | 6271 | 6447 | 150 | 48.7% | 0.5177 | 35.3% | -0.7706 |
| D7 | Multi-exchange Consensus | - | 5835 | 6883 | 150 | 45.3% | 0.2753 | 33.3% | -0.8967 |
| D8 | Chainlink Lag / Update Risk | - | 7077 | 5641 | 150 | 55.0% | 0.6149 | 38.9% | -0.6305 |

## D6 Mean Reversion Risk

- **d6_high_count**: `1863`
- **d6_medium_count**: `4328`
- **d6_low_count**: `6527`
- **win_rate_by_d6_risk_level**: `{'low': 0.35294117647058826, 'medium': 1.0, 'unknown': 0.5172413793103449}`
- **avg_pnl_by_d6_risk_level**: `{'low': -0.7705823529411765, 'medium': 1.75, 'unknown': -0.20873793103448277}`
- **blocked_by_mean_reversion_count**: `1863`
- **mean_reversion_risk_high_count**: `1863`
- **distance_shrinking_true_count**: `6696`
- **win_rate_when_distance_shrinking_true**: `0.4000`
- **avg_pnl_when_distance_shrinking_true**: `-0.7200`

## D7 Multi-Exchange Consensus

- **d7_active_count**: `5835`
- **d7_neutral_count**: `6883`
- **d7_insufficient_data_count**: `0`
- **d7_neutral_rate**: `0.5349`
- **d7_insufficient_data_rate**: `0.0000`
- **win_rate_when_d7_active**: `0.3333`
- **avg_pnl_when_d7_active**: `-0.8967`
- **win_rate_when_d7_neutral**: `0.6667`
- **avg_pnl_when_d7_neutral**: `0.7000`

## D1/D2 Correlation

- **sample_count**: `12718`
- **pearson**: `0.9813`
- **warning**: `True`

## Entry Price Buckets

| bucket | trades | wins | losses | win rate | total pnl | avg pnl |
|---|---:|---:|---:|---:|---:|---:|
| <0.30 | 3 | 1 | 2 | 33.3% | 1.4000 | 0.4667 |
| 0.30-0.40 | 3 | 0 | 3 | 0.0% | -5.2500 | -1.7500 |
| 0.40-0.50 | 7 | 0 | 7 | 0.0% | -16.6969 | -2.3853 |
| 0.50-0.60 | 16 | 11 | 5 | 68.8% | 10.1465 | 0.6342 |
| 0.60-0.65 | 18 | 10 | 8 | 55.6% | -7.0029 | -0.3890 |
| >0.65 | 0 | 0 | 0 | - | - | - |
| unknown | 0 | 0 | 0 | - | - | - |

## Direction Breakdown

| group | trades | wins | losses | win rate | total pnl | avg pnl | avg entry |
|---|---:|---:|---:|---:|---:|---:|---:|
| UP | 46 | 21 | 25 | 45.7% | -19.8033 | -0.4305 | 0.5426 |
| DOWN | 1 | 1 | 0 | 100.0% | 2.4000 | 2.4000 | 0.5200 |

## Entry Price Bucket by Direction

| group | trades | wins | losses | win rate | total pnl | avg pnl | avg entry |
|---|---:|---:|---:|---:|---:|---:|---:|
| <0.30 / UP | 3 | 1 | 2 | 33.3% | 1.4000 | 0.4667 | 0.2400 |
| <0.30 / DOWN | 0 | 0 | 0 | - | - | - | - |
| 0.30-0.40 / UP | 3 | 0 | 3 | 0.0% | -5.2500 | -1.7500 | 0.3500 |
| 0.30-0.40 / DOWN | 0 | 0 | 0 | - | - | - | - |
| 0.40-0.50 / UP | 7 | 0 | 7 | 0.0% | -16.6969 | -2.3853 | 0.4771 |
| 0.40-0.50 / DOWN | 0 | 0 | 0 | - | - | - | - |
| 0.50-0.60 / UP | 15 | 10 | 5 | 66.7% | 7.7465 | 0.5164 | 0.5633 |
| 0.50-0.60 / DOWN | 1 | 1 | 0 | 100.0% | 2.4000 | 2.4000 | 0.5200 |
| 0.60-0.65 / UP | 18 | 10 | 8 | 55.6% | -7.0029 | -0.3890 | 0.6333 |
| 0.60-0.65 / DOWN | 0 | 0 | 0 | - | - | - | - |
| >0.65 / UP | 0 | 0 | 0 | - | - | - | - |
| >0.65 / DOWN | 0 | 0 | 0 | - | - | - | - |
| unknown / UP | 0 | 0 | 0 | - | - | - | - |
| unknown / DOWN | 0 | 0 | 0 | - | - | - | - |

## D7 by Direction

| group | trades | wins | losses | win rate | total pnl | avg pnl | avg entry |
|---|---:|---:|---:|---:|---:|---:|---:|
| active / UP | 15 | 5 | 10 | 33.3% | -13.4499 | -0.8967 | 0.5127 |
| active / DOWN | 0 | 0 | 0 | - | - | - | - |
| neutral / UP | 3 | 2 | 1 | 66.7% | 2.1000 | 0.7000 | 0.5267 |
| neutral / DOWN | 0 | 0 | 0 | - | - | - | - |
| missing / UP | 28 | 14 | 14 | 50.0% | -8.4534 | -0.3019 | 0.5603 |
| missing / DOWN | 1 | 1 | 0 | 100.0% | 2.4000 | 2.4000 | 0.5200 |

## D6 Distance Shrinking Breakdown

| group | trades | wins | losses | win rate | total pnl | avg pnl | avg entry |
|---|---:|---:|---:|---:|---:|---:|---:|
| true / UP / low | 4 | 1 | 3 | 25.0% | -5.3499 | -1.3375 | 0.5175 |
| true / UP / medium | 1 | 1 | 0 | 100.0% | 1.7500 | 1.7500 | 0.6500 |
| true / UP / high | 0 | 0 | 0 | - | - | - | - |
| true / UP / unknown | 0 | 0 | 0 | - | - | - | - |
| true / DOWN / low | 0 | 0 | 0 | - | - | - | - |
| true / DOWN / medium | 0 | 0 | 0 | - | - | - | - |
| true / DOWN / high | 0 | 0 | 0 | - | - | - | - |
| true / DOWN / unknown | 0 | 0 | 0 | - | - | - | - |
| false / UP / low | 13 | 5 | 8 | 38.5% | -7.7500 | -0.5962 | 0.5038 |
| false / UP / medium | 0 | 0 | 0 | - | - | - | - |
| false / UP / high | 0 | 0 | 0 | - | - | - | - |
| false / UP / unknown | 0 | 0 | 0 | - | - | - | - |
| false / DOWN / low | 0 | 0 | 0 | - | - | - | - |
| false / DOWN / medium | 0 | 0 | 0 | - | - | - | - |
| false / DOWN / high | 0 | 0 | 0 | - | - | - | - |
| false / DOWN / unknown | 0 | 0 | 0 | - | - | - | - |
| unknown / UP / low | 0 | 0 | 0 | - | - | - | - |
| unknown / UP / medium | 0 | 0 | 0 | - | - | - | - |
| unknown / UP / high | 0 | 0 | 0 | - | - | - | - |
| unknown / UP / unknown | 28 | 14 | 14 | 50.0% | -8.4534 | -0.3019 | 0.5603 |
| unknown / DOWN / low | 0 | 0 | 0 | - | - | - | - |
| unknown / DOWN / medium | 0 | 0 | 0 | - | - | - | - |
| unknown / DOWN / high | 0 | 0 | 0 | - | - | - | - |
| unknown / DOWN / unknown | 1 | 1 | 0 | 100.0% | 2.4000 | 2.4000 | 0.5200 |

## D1/D2 Directional Correlation

- **all_decisions**: sample_count=`12718`, pearson=`0.9813`, warning=`True`
- **up_decisions**: sample_count=`5313`, pearson=`0.5531`, warning=`False`
- **down_decisions**: sample_count=`7400`, pearson=`0.6794`, warning=`False`
- **traded_decisions**: sample_count=`18`, pearson=`0.6485`, warning=`False`
- **losing_trades**: sample_count=`11`, pearson=`-`, warning=`False`
- **winning_trades**: sample_count=`7`, pearson=`0.7624`, warning=`True`

## Worst Trade Diagnostics

| market | direction | entry | pnl | success | actual | decision | D1 | D2 | D6 risk | shrinking | D7 state | D7 | confidence | gap | reject | final block |
|---|---|---:|---:|---|---|---|---:|---:|---|---|---|---:|---:|---:|---|---|
| btc-updown-5m-1780262100 | UP | 0.6500 | -3.2500 | False | UNKNOWN | - | - | - | unknown | - | missing | - | - | - | - | - |
| btc-updown-5m-1780275000 | UP | 0.6500 | -3.2500 | False | UNKNOWN | - | - | - | unknown | - | missing | - | - | - | - | - |
| btc-updown-5m-1780323300 | UP | 0.6500 | -3.2500 | False | UNKNOWN | 2026-06-01T14:17:48.420088423Z | 2.0000 | 1.4000 | low | False | active | 0.6000 | 0.9030 | 9.0300 |  | - |
| btc-updown-5m-1780282200 | UP | 0.6300 | -3.1500 | False | UNKNOWN | - | - | - | unknown | - | missing | - | - | - | - | - |
| btc-updown-5m-1780282500 | UP | 0.6300 | -3.1500 | False | UNKNOWN | - | - | - | unknown | - | missing | - | - | - | - | - |
| btc-updown-5m-1780328400 | UP | 0.6300 | -3.1500 | False | UNKNOWN | 2026-06-01T15:42:51.319539319Z | 2.0000 | 1.4000 | low | False | active | 0.6000 | 0.8355 | 8.3550 |  | - |
| btc-updown-5m-1780253700 | UP | 0.6100 | -3.0500 | False | UNKNOWN | - | - | - | unknown | - | missing | - | - | - | - | - |
| btc-updown-5m-1780256400 | UP | 0.6100 | -3.0500 | False | UNKNOWN | - | - | - | unknown | - | missing | - | - | - | - | - |
| btc-updown-5m-1780371000 | UP | 0.6000 | -3.0000 | False | UNKNOWN | 2026-06-02T03:32:30.273964716Z | 1.0972 | 1.4000 | low | True | active | 0.6000 | 0.7452 | 7.4522 |  | - |
| btc-updown-5m-1780382400 | UP | 0.6000 | -3.0000 | False | UNKNOWN | 2026-06-02T06:42:30.274172746Z | 0.7527 | 1.4000 | low | False | active | 0.6000 | 0.6787 | 6.7867 |  | - |
| btc-updown-5m-1780259400 | UP | 0.5600 | -2.8000 | False | UNKNOWN | - | - | - | unknown | - | missing | - | - | - | - | - |
| btc-updown-5m-1780274100 | UP | 0.5500 | -2.7500 | False | UNKNOWN | - | - | - | unknown | - | missing | - | - | - | - | - |
| btc-updown-5m-1780259100 | UP | 0.5300 | -2.6500 | False | UNKNOWN | - | - | - | unknown | - | missing | - | - | - | - | - |
| btc-updown-5m-1780250700 | UP | 0.4994 | -2.4970 | False | UNKNOWN | - | - | - | unknown | - | missing | - | - | - | - | - |
| btc-updown-5m-1780277700 | UP | 0.4900 | -2.4500 | False | UNKNOWN | - | - | - | unknown | - | missing | - | - | - | - | - |

## Suspicious 0.30-0.50 Entry Cluster

| market | direction | entry | pnl | success | actual | decision | D1 | D2 | D6 risk | shrinking | D7 state | D7 | confidence | gap | reject | final block |
|---|---|---:|---:|---|---|---|---:|---:|---|---|---|---:|---:|---:|---|---|
| btc-updown-5m-1780250700 | UP | 0.4994 | -2.4970 | False | UNKNOWN | - | - | - | unknown | - | missing | - | - | - | - | - |
| btc-updown-5m-1780277700 | UP | 0.4900 | -2.4500 | False | UNKNOWN | - | - | - | unknown | - | missing | - | - | - | - | - |
| btc-updown-5m-1780251900 | UP | 0.4800 | -2.4000 | False | UNKNOWN | - | - | - | unknown | - | missing | - | - | - | - | - |
| btc-updown-5m-1780254000 | UP | 0.4800 | -2.4000 | False | UNKNOWN | - | - | - | unknown | - | missing | - | - | - | - | - |
| btc-updown-5m-1780317000 | UP | 0.4800 | -2.4000 | False | UNKNOWN | 2026-06-01T12:32:48.084388693Z | 1.8201 | 1.4000 | low | False | active | 0.6000 | 0.8175 | 8.1751 |  | - |
| btc-updown-5m-1780324200 | UP | 0.4700 | -2.3499 | False | UNKNOWN | 2026-06-01T14:32:50.303490046Z | 2.0000 | 1.4000 | low | True | active | 0.6000 | 0.7680 | 7.6800 |  | - |
| btc-updown-5m-1780327200 | UP | 0.4400 | -2.2000 | False | UNKNOWN | 2026-06-01T15:22:45.512828953Z | 1.5041 | 1.4000 | low | True | active | 0.6000 | 0.8534 | 8.5341 |  | - |
| btc-updown-5m-1780327500 | UP | 0.3900 | -1.9500 | False | UNKNOWN | 2026-06-01T15:28:16.288417397Z | 2.0000 | 1.4000 | low | False | neutral | 0.0000 | 0.7755 | 7.7550 |  | - |
| btc-updown-5m-1780365000 | UP | 0.3400 | -1.7000 | False | UNKNOWN | 2026-06-02T01:53:44.285984305Z | 2.0000 | 1.4000 | low | False | active | 0.6000 | 0.8355 | 8.3550 |  | - |
| btc-updown-5m-1780328100 | UP | 0.3200 | -1.6000 | False | UNKNOWN | 2026-06-01T15:38:15.889452545Z | 1.6076 | 1.4000 | low | False | active | 0.6000 | 0.6018 | 6.0176 |  | - |

## Reject Reasons

- `spot_chainlink_disagreement`: 4471
- `ask_too_high`: 3708
- `insufficient_side_score`: 2646
- `mean_reversion_risk_high`: 1863
- `invalid_price_to_beat`: 120
- `rtds_unhealthy`: 30
- `unknown_result`: 6
- `no_selected_signal`: 5
- `risk_gate_blocked`: 4

## Conclusion Notes

- D1/D2 contributions are strongly correlated; continue observing potential overlap.
- This report is diagnostic only and does not recommend automatic factor weight changes.
