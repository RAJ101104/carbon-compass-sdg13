 Carbon Compass

A personal carbon footprint tracker I built for my AI / Web Development final project, addressing UN Sustainable Development Goal 13: Climate Action.

Most carbon calculators just give you one number and generic advice like "use less plastic." I wanted to build something that actually tells you *which* of your habits is the biggest problem and *how much* changing it would actually save — backed by a simple AI recommendation engine instead of generic tips.

 What it does

You enter a few details about your everyday life — how much you drive, your electricity use, your diet, how often you fly, and your waste habits. The app calculates your yearly carbon footprint from that, shows you where it's coming from, and then ranks the changes that would help the most, with an estimated saving in kg of CO2 for each one. There's also a small chat assistant you can ask questions like "what's my biggest source?" and it answers using your actual numbers, not a generic script.

 Features

- Input form with sliders and dropdowns for transport, electricity, diet, flights, and waste, including a choice of electricity grid (India, global average, renewable-heavy, USA) so the numbers are localized rather than US/UK-default.
- A radial gauge ("the Carbon Dial") showing your total footprint against three reference lines: a 1.5°C-aligned personal target, the India average, and the global average.
- A breakdown of exactly how many kg and what percentage each category contributes.
- A rule-based AI engine that ranks your biggest emission sources and suggests a specific action for each, with an estimated annual saving.
- "Ask the Compass" — a small chat box that answers questions about your own results.
- A goal slider and a log so you can save multiple readings and see a trend line over time.
- Everything runs in the browser. No server, no account, no data leaves your device.

 How to use the app

1. Open `index.html` in your browser — double-clicking the file is enough, nothing to install.
2. Adjust the sliders and dropdowns under "Take a reading" (transport, electricity, diet, flights, waste), or just leave the default values if you want a quick example.
3. Click **Calculate footprint**.
4. The page scrolls down to "Your reading" — the dial shows your total footprint in tonnes of CO2 per year, and the bars next to it show which category is contributing the most.
5. Scroll down to "Where to act first" to see the three AI-generated recommendations, ranked by impact.
6. Try "Ask the Compass" — type a question such as "what's my biggest source?" or "how do I cut my transport footprint?" and it will answer using your own numbers.
7. Under "Set a target, track your trend," move the reduction-target slider to see what a percentage cut means in tonnes, then click **Save this reading to my log**. Change a slider, recalculate, and save again to watch the trend line update.






 Tech stack

- HTML5, CSS3 (custom properties, Grid), vanilla JavaScript — no frameworks, no build tools
- Hand-built SVG for the gauge, bar charts, and trend sparkline, so there's no charting library dependency
- A rule-based recommendation and keyword-matching engine for the AI layer
- Browser localStorage for the reading log
- Google Fonts: Fraunces, Inter, JetBrains Mono

 

## Future scope

- Swap the rule-based assistant for a real generative model (Anthropic or OpenAI API) through a small backend
- More granular emission factors — vehicle/fuel type, live regional grid-mix data
- Auto-fill travel data through a maps/transit API instead of manual sliders
- A native mobile app with reminders
- Classroom or office group challenges with opt-in shared leaderboards
- Multi-language support
- An exportable PDF footprint report

## License

MIT — see [LICENSE](LICENSE).
