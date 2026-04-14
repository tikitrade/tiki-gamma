# TradingView Publication Description

Last updated: 2026-03-23

---

## Title

Tiki Gamma — Options Dealer Levels for Futures & Index Traders

## Short Description (for search/preview)

Real-time options dealer hedging levels — gamma walls, regime filter, volatility triggers — on your TradingView chart. Free and open source.

## Full Description
Tiki Gamma maps the options dealer hedging levels that shape intraday price action — directly on your chart.

Options dealers hedge trillions in exposure every session. When price approaches a significant strike, they are mechanically forced to buy or sell the underlying on every tick. These flows are systematic, large, and predictable enough to define the structural support and resistance that institutional desks watch as primary reference points.

This indicator draws those levels. It does not repaint. It is not a lagging signal. It visualizes the market structure derived from the live options chain.

[b]What It Draws[/b]

[b]Call Walls & Put Walls[/b] — Overhead zones where dealer selling is heaviest. Below-market zones where dealer buying provides structural support. Call walls resist more consistently; put walls, when they break, break hard. Line thickness scales with strength so the dominant level is immediately visible.

[b]Zero Gamma Flip[/b] — The single most important regime filter in modern markets. Above it, dealers trade against every move — mean-reverting. Below it, dealers trade with every move — amplifying. One line changes how you size, hold, and manage risk.

[b]Expert Configuration[/b] (Signal-to-Noise Ratio) — Ships with optimized configuration for high-conviction trading. We recommend limiting Walls and Absolute Gamma to 3 levels each at 80%+ strength to filter out noise, while keeping Large Gamma at a 5-level, 50% strength threshold to catch secondary intraday pivots.

[b]Gamma Transition Band[/b] (Experimental) — The contested zone around the flip where dealer positioning is mixed. Price action inside this band is inherently noisier. These levels are currently in experimental beta.

[b]Key Gamma Strike & Large Gamma [/b]— The market's gravitational centers. In drift sessions, price magnetizes toward them. In trending sessions, they become checkpoint S/R. Optional strength percentages and GEX magnitude labels show which levels carry real weight.

[b]Vanna Inflection[/b] — Where an IV expansion triggers forced delta rehedging independent of price movement. The level that matters most on gap opens and VIX events.

[b]Speed Trap[/b] — Where a small downward move creates disproportionate dealer selling. The level that turns a pullback into a flush.

[b]Max Pain[/b] — The settlement gravity point. The zone expands automatically near close as charm-driven delta unwinding strengthens into expiration — the mechanism behind end-of-day pinning behavior.

[b]Expected / Implied Move Bands[/b] — 1-SD and 2-SD statistical envelopes. Inside the box: mean reversion is plausible. Outside it: respect the move.

[b]Visual Design[/b]

[list]
[*][b]Regime Background[/b] — Chart can be configured to tint teal above the gamma flip (stabilizing), magenta below (amplifying). Off by default to minimize clutter.
[*][b]Strength-Scaled Lines & Opacity[/b] — Dominant levels draw thicker and more opaque. Weaker levels fade. Hierarchy is visible without reading a single label.
[*][b]HUD Dashboard[/b] — Compact overlay showing current regime, distance to nearest walls in implied-move units (sigma), and futures basis shift.
[*][b]Proximity Highlighting[/b] — Zone opacity increases when price enters a level. The active level always stands out.
[*][b]Max Pain Expansion[/b] — The max pain zone grows as charm effects strengthen into the close, reflecting real-time gravitational pull.
[*][b]Price Axis Tags[/b] — Every level is tagged on the price axis for quick reference without chart clutter.
[*][b]Futures Basis Shift[/b] — SPX/NDX levels mapped accurately onto ES/NQ charts. When in Auto mode, the indicator dynamically calculates the exact, real-time basis offset using prior close data to ensure perfect, stable alignment. If the ticker is unmapped, it automatically falls back to your initially pasted Basis Shift.
[/list]

[b]Settings & Configuration[/b]

The indicator features deep customisation via its settings panel, grouped for ease of use:

[list]
[*][b]Visibility[/b] — Toggle individual level types (Walls, GEX nodes, Vanna, Speed Trap, etc.), the HUD Dashboard, and Price Axis Labels. Choose between Level names, Prices, or both for on-chart labels.
[*][b]Style[/b] — Adjust base Line Width and enable Strength scaling for width/opacity. Toggle GEX Magnitude ($) and Vol Resilience (↑/↓) arrows in labels. Select Label Alignment (Left vs Last Bar) and Format (Full vs Abbreviated). Configure Display Timezone for timestamped levels.
[*][b]Level Filters[/b] — Fine-tune signal clarity by setting global and per-type "Min Strength %" thresholds. Use the "Max Total Levels" cap to limit the total number of lines drawn near price.
[*][b]Colors & Opacity[/b] — Customise the color for every level category. Global sliders control base opacity for lines and shaded influence zones.
[*][b]Visual Effects & Advanced[/b] — Configure Regime Background colors and opacity. Customise Advanced Max Pain settings, including the close-time target and the growth window for end-of-day expansion.
[/list]

[b]How It Works[/b]

Paste the full level payload from Tikitrade into the indicator's text input. Each level accepts optional metadata — strength, vol resilience, and GEX magnitude — so the indicator reflects the full depth of the pipeline output, not just price levels.

Free daily SPX/ES reference levels are available at [url=https://tikitrade.com/gamma]tikitrade.com/gamma[/url]. For real-time levels refreshed from the live options chain across all supported symbols and professional composite data (SPX+SPY, NDX+QQQ), a Tikitrade membership is required at [url=https://tikitrade.com]tikitrade.com[/url].

[b]Open Source[/b]

Full source is published openly. Read it, fork it, learn from it. Every level type is documented in the script header with the dealer mechanics that drive it. Contribute via Github here: [url=https://github.com/tikitrade/tiki-gamma]github.com/tikitrade/tiki-gamma[/url]

---

**Keywords** (not displayed, for search optimization in the description body):
gamma exposure, GEX, dealer hedging, options flow, gamma flip, zero gamma, call wall, put wall, max pain, vanna, speed trap, implied move, expected move, futures, ES, NQ, SPX, NDX, options levels, dealer positioning, gamma squeeze, open source

## Tags

Options, Gamma, GEX, Futures, Dealer Hedging, Support Resistance, SPX, ES, Market Structure

## Publication Notes

- Publish as **open source** (eligible for Staff Picks and Editor's Picks)
- Screenshot: ES chart, teal regime background, call wall rejection overhead, key gamma strike visible, HUD active
- Respond to every comment in the first 48 hours (algorithmic ranking signal)
- Do not mention competitors by name
