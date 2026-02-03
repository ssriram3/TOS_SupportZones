# Trading Zones - ThinkorSwim Script

## Overview
This script plots key support and resistance levels on your 1D 5min chart to help identify potential trading zones. It displays the previous day's high/low and 5-day high/low levels with built-in filtering for erroneous price data.

## Zones Created

### Previous Day Levels
**Previous Day High (PDH)** - Cyan solid line
- Represents yesterday's highest price point
- Often acts as resistance during the current trading session
- Breakouts above PDH can signal bullish momentum
- Failed breaks may indicate rejection and potential reversal

**Previous Day Low (PDL)** - Magenta solid line
- Represents yesterday's lowest price point
- Often acts as support during the current trading session
- Breaks below PDL can signal bearish momentum
- Bounces off PDL may indicate buying interest

### 5-Day Levels
**5-Day High (5DH)** - Yellow dashed line
- The highest price point over the last 5 trading days
- Represents a significant resistance zone
- Major breakouts above this level often indicate strong bullish trends
- Multiple tests without breaking can create strong resistance

**5-Day Low (5DL)** - Orange dashed line
- The lowest price point over the last 5 trading days
- Represents a significant support zone
- Breaks below this level often indicate strong bearish trends
- Multiple tests without breaking can create strong support

## Trading Applications

### Support & Resistance Trading
- Watch for price reactions at these levels (bounces, rejections, consolidation)
- Strong reactions confirm the zone's validity
- Weak reactions may signal the level is losing importance

### Breakout Trading
- PDH/PDL breakouts: Shorter-term momentum plays
- 5DH/5DL breakouts: Stronger conviction, potential for larger moves
- Look for volume confirmation on breakouts

### Range Trading
- Trade between PDH and PDL for intraday ranges
- Trade between 5DH and 5DL for swing ranges
- Fade extremes when price approaches these levels

### Risk Management
- Use these levels as logical stop-loss placement zones
- PDH/PDL for tighter intraday stops
- 5DH/5DL for wider swing trade stops

## Special Features

### Anomaly Filtering
The script automatically filters out "fat-finger" trades or erroneous data:
- Detects price spikes >30% from the previous day's close
- Substitutes anomalous data with the prior period's value
- Ensures clean, tradeable levels without outliers

### Visual Design
- **Line thickness**: All lines set to weight 4 for clear visibility
- **Solid lines**: Previous day levels (more frequent tests)
- **Dashed lines**: 5-day levels (major zones)
- **Color coding**: Easy identification at a glance
- **Labels**: Current values displayed at the top of the chart

## Best Practices

1. **Confluence**: Levels are most powerful when multiple zones align (e.g., PDH near 5DH)
2. **Context**: Consider overall market trend and volatility
3. **Time of Day**: Early session often tests previous day levels
4. **Volume**: Confirm breakouts/breakdowns with volume analysis
5. **Multiple Timeframes**: Use these intraday levels alongside higher timeframe support/resistance

## Installation
1. Open ThinkorSwim
2. Go to Studies → Edit Studies → New
3. Paste the script code
4. Apply to your 1D 5min chart
5. Customize colors/thickness in the script if desired

---

*Note: These levels are reference points, not guaranteed trading signals. Always use proper risk management and combine with your trading strategy.*