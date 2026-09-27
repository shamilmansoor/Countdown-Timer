# ⏱ Countdown Timer

A sleek, single-file countdown timer web app with a retro sci-fi / HUD aesthetic — glowing accents, scan-line effects, a grid overlay, and dynamic color states that shift as time runs out. Built entirely with vanilla HTML, CSS, and JavaScript — no dependencies, no build step.

## Features

- **Custom duration input** — set hours, minutes, and seconds (HH:MM:SS)
- **Start / Pause / Reset controls**
- **Optional starting buzzer** — plays a rising three-tone chime when the timer begins
- **Optional pre-start cooldown** — an adjustable 1–10 second "starting in…" countdown overlay with beeps before the main timer starts
- **Dynamic visual states** — the background, glow, and timer color shift through distinct themes as the timer progresses:
  - **Countdown** (pre-start cooldown) — cyan
  - **Running** — green
  - **Warning** (≤25% of time remaining) — orange
  - **Critical** (≤10 seconds remaining) — red, with a pulsing flash
  - **Done** — red alert flash with an end buzzer
- **Audio alerts** — Web Audio API–generated tick warnings, countdown beeps, and an end-of-timer buzzer, all with an adjustable volume slider
- **Auto-scaling display** — the time text automatically resizes to fit the card at any screen size
- **Responsive layout** — adapts cleanly from desktop down to small mobile screens

## Getting Started

No installation or build tools required.

1. Clone the repository:
   ```bash
   git clone https://github.com/shamilmansoor/Countdown-Timer.git
   ```
2. Open `index.html` in any modern web browser.

That's it — the timer runs entirely client-side.

## Usage

1. Enter the desired **hours**, **minutes**, and **seconds** in the input fields.
2. (Optional) Toggle **Starting Buzzer** to play a sound when the timer starts.
3. (Optional) Toggle **Cooldown Before Start** and adjust the delay slider to add a countdown before the timer begins.
4. Click **Start** to begin the countdown.
5. Use **Pause** to halt the timer, or **Reset** to clear it and set a new duration.
6. Adjust the **Volume** slider to control alert sound levels.

## Tech Stack

- **HTML5**
- **CSS3** (custom properties, animations, responsive `clamp()`-based sizing)
- **Vanilla JavaScript** (DOM manipulation, `setInterval`/`setTimeout` timing, Web Audio API for sound generation)
- **Google Fonts** — [Share Tech Mono](https://fonts.google.com/specimen/Share+Tech+Mono) and [Orbitron](https://fonts.google.com/specimen/Orbitron)

## Project Structure

```
Countdown-Timer/
└── index.html   # Entire app: markup, styles, and logic in one file
```

## Browser Support

Works in any modern browser with support for the Web Audio API and CSS custom properties (Chrome, Firefox, Edge, Safari).

## License

No license file is currently included in this repository. Add one (e.g., MIT) if you intend for others to reuse this code.

## Author

[shamilmansoor](https://github.com/shamilmansoor)
