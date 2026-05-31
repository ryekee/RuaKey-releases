<div align="center">

<img src="https://raw.githubusercontent.com/ryekee/RuaKey-releases/main/docs/dashboard.png" width="760" alt="RuaKey dashboard" />

# ⌨️ RuaKey

**A privacy-first keyboard analytics app for macOS.**
See *how* you type — without ever recording *what* you type.

[![Download latest](https://img.shields.io/github/v/release/ryekee/RuaKey-releases?label=Download&style=for-the-badge&color=fab387)](https://github.com/ryekee/RuaKey-releases/releases/latest)

macOS 14+ · Apple Silicon · lives in your menu bar

</div>

---

RuaKey turns your keyboard (and mouse) activity into clean, **local** insights: how fast you type, which keys and shortcuts you lean on, which apps eat your keystrokes, and how it all trends over time.

It counts **metadata only** — key categories, per-key tallies, modifier combos — all aggregated **by day**. It never stores the order or timing of keystrokes, so it physically **cannot reconstruct anything you typed**.

## 🔒 Privacy is the whole point

- **Your input never leaves this Mac.** No telemetry, no analytics SDKs, no cloud sync.
- **No keystroke content, ever** — only categories and daily per-key counts, never *(time, key)* sequences.
- **Per physical keyboard**, via Apple's `IOHIDManager` — data is grouped by device, not skimmed off a system-wide event stream.
- The *only* network the app makes is checking GitHub for updates — and you can turn it off.

> The stored database has no text fields. There's simply no way to recover words from daily category counts.

## ✨ What you get

- **📊 Dashboard** — today / 7-day / 30-day / lifetime totals, live & peak KPM, input speed (WPM), backspace rate, active streaks, hour-of-day & day-of-week patterns, and a year activity calendar.
- **⌨️ Keyboard heatmap** — your most-pressed keys on a real board, across layouts: **MacBook · 75% · TKL · Alice · HHKB**.
- **🖱️ Mouse** — click & scroll counts and a smooth per-display click heatmap (coordinates are quantized on capture — raw positions never touch disk).
- **📱 Per-app** — which apps get your keystrokes and clicks.
- **📈 7-day comparison** — every stat shows today vs. your last 7 days.
- **🎚️ Floating HUD** — an optional live strip (KPM · current key · today's count) that auto-shows while you type and slips out of the way when your cursor comes near.
- **🎉 Milestone Confetti** — a full-screen celebration when you set a new 7-day record.
- **🔄 Auto-update** — new versions install themselves.

All in a dark terminal/dashboard aesthetic — amber + green, Departure Mono, dense machine-readout panels.

## 📥 Install

1. **[Download the latest `.dmg`](https://github.com/ryekee/RuaKey-releases/releases/latest)** and drag **RuaKey** into Applications.
2. First launch: **right-click → Open** to pass Gatekeeper (the app is ad-hoc signed, not notarized).
3. Grant **Input Monitoring** when asked, then **quit and relaunch** — macOS requires a restart to enable it.

After 0.3.0, updates arrive automatically; no need to come back here.

---

<div align="center">
<sub>RuaKey records counts, not content. Your words stay yours.</sub>
</div>
