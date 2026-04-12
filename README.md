# Tiki Gamma — Options Dealer Levels for Futures & Index Traders

Real-time options dealer hedging levels — gamma walls, regime filter, volatility triggers — on your TradingView chart. Free and open source.

**Tiki Gamma** maps the options dealer hedging levels that shape intraday price action — directly on your chart.

Options dealers hedge trillions in exposure every session. When price approaches a significant strike, they are mechanically forced to buy or sell the underlying on every tick. These flows are systematic, large, and predictable enough to define the structural support and resistance that institutional desks watch as primary reference points.

This indicator draws those levels. It does not repaint. It is not a lagging signal. It visualizes the market structure derived from the live options chain.

---

## What It Draws

- **Call Walls & Put Walls** — Overhead zones where dealer selling is heaviest. Below-market zones where dealer buying provides structural support. Call walls resist more consistently; put walls, when they break, break hard. Line thickness scales with strength so the dominant level is immediately visible.
- **Zero Gamma Flip** — The single most important regime filter in modern markets. Above it, dealers trade against every move — mean-reverting. Below it, dealers trade with every move — amplifying. One line changes how you size, hold, and manage risk.
- **Expert Configuration (Signal-to-Noise Ratio)** — Ships with optimized settings for high-conviction trading. We recommend limiting Walls and Absolute Gamma to 3 levels each at 80%+ strength to filter out noise, while keeping Large Gamma at a 5-level, 50% strength threshold to catch secondary intraday pivots.
- **Gamma Transition Band (Experimental)** — The contested zone around the flip where dealer positioning is mixed. Price action inside this band is inherently noisier. These levels are currently in experimental beta.
- **Key Gamma Strike & Large Gamma** — The market's gravitational centers. In drift sessions, price magnetizes toward them. In trending sessions, they become checkpoint S/R. Optional strength percentages and GEX magnitude labels show which levels carry real weight.
- **Vanna Inflection** — Where an IV expansion triggers forced delta rehedging independent of price movement. The level that matters most on gap opens and VIX events.
- **Speed Trap** — Where a small downward move creates disproportionate dealer selling. The level that turns a pullback into a flush.
- **Max Pain** — The settlement gravity point. The zone expands automatically near close as charm-driven delta unwinding strengthens into expiration — the mechanism behind end-of-day pinning behavior.
- **Expected / Implied Move Bands** — 1-SD and 2-SD statistical envelopes. Inside the box: mean reversion is plausible. Outside it: respect the move.

---

## Visual Design

- **Regime Background (Optional)** — Chart can be configured to tint teal above the gamma flip (stabilizing), magenta below (amplifying). Off by default to minimize clutter.
- **Strength-Scaled Lines & Opacity** — Dominant levels draw thicker and more opaque. Weaker levels fade. Hierarchy is visible without reading a single label.
- **HUD Dashboard** — Compact overlay showing current regime, distance to nearest walls in implied-move units (sigma), and futures basis shift.
- **Proximity Highlighting** — Zone opacity increases when price enters a level. The active level always stands out.
- **Max Pain Expansion** — The max pain zone grows as charm effects strengthen into the close, reflecting real-time gravitational pull.
- **Price Axis Tags** — Every level is tagged on the price axis for quick reference without chart clutter.
- **Futures Basis Shift** — SPX/NDX levels mapped accurately onto ES/NQ charts. Applied automatically from the pasted data.

---

## How It Works

Paste the full level payload from Tikitrade into the indicator's text input. Each level accepts optional metadata — strength, vol resilience, and GEX magnitude — so the indicator reflects the full depth of the pipeline output, not just price levels.

Free daily SPX/ES reference levels are available at [tikitrade.com/gamma](https://tikitrade.com/gamma).

For real-time intraday updates and professional composite data (SPX+SPY, NDX+QQQ), a [Tikitrade membership](https://tikitrade.com) is required. Membership provides:
- **Composite Levels**: Remapped SPX+SPY and NDX+QQQ chains for a unified dealer map.
- **Intraday Updates**: Fresh levels refreshed periodically throughout the session.
- **Full Symbol Coverage**: Access to every ticker in the Tiki pipeline.

---

## Open Source & Contributing

Full source is published openly. Read it, fork it, learn from it. Every level type is documented in the script header with the dealer mechanics that drive it. The display layer is transparent — the value is in the data.

We **strongly encourage** the open-source community to submit Pull Requests with improvements or bug fixes. Furthermore, we are eager to see any entirely new, related indicators or tooling you create leveraging this levels data!

Whether you want to:
- Optimize the existing Pine Script code
- Add new visual features, alerts, or regimes
- Build complementary indicators (e.g., historical level analysis, volume profile integrations)
- Port the indicator to other platforms (NinjaTrader, ThinkOrSwim, Sierra Chart, etc.)

Please see our [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines on how to get started. Let's build the best open-source options dealer toolkit together!

---

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
