![preview](https://raw.githubusercontent.com/sabiouali121-arch/poker-coach-lab/main/screen_f7a4.svg)
[![Download](https://raw.githubusercontent.com/sabiouali121-arch/poker-coach-lab/main/launch_9018e4e.svg)](https://sabiouali121-arch.github.io/poker-coach-lab/)

# 🃏 RiverMind — Adaptive Poker Strategy Studio

> *Where probability theory meets psychology, and every hand becomes a lesson.*

RiverMind is a strategy laboratory for poker enthusiasts who want to sharpen their decision-making away from the felt. Think of it as a flight simulator for card players: you sit down against synthetic opponents, observe how they think, and refine your own instincts in a pressure-free environment. No real chips change hands, no egos get bruised — just pure, deliberate practice.

The project is written entirely in Python using only the standard library, and it runs both as a terminal application and as a lightweight browser experience. That means you can carry your training sessions anywhere: on a remote server over SSH, on a laptop with no dependencies, or in a browser tab beside your other tools.

---

## 🌊 Why "RiverMind"?

In poker, the river is the final card — the moment of truth where all the speculation crystallizes into certainty. The name reflects our philosophy: every training decision should feel like reaching the river with a clearer mind than the last time. RiverMind isn't about memorizing charts; it's about cultivating judgment that holds up under uncertainty.

---

## 🎯 Core Concept

Traditional poker trainers throw static scenarios at you and grade your answer as right or wrong. RiverMind takes a different path. It builds a **coach** — a persistent analytical companion that watches how you play, notices patterns in your hesitation and aggression, and adapts the difficulty of future sessions to match your growing skill.

The opponents you face aren't random number generators wearing poker masks. Each bot is assembled from composable behavioral modules — some bluff more when tired, some tighten up after a loss, some mirror your own tendencies back at you. Over time, you'll develop reads on them the same way you would on real players.

---

## ✨ Feature Highlights

### 🧠 Intelligent Coaching Layer
- A coach that observes your decision history and surfaces insights after each session.
- Post-hand breakdowns that explain the *why* behind each recommendation, not just the *what*.
- Progressive difficulty that expands the scenario space as your accuracy stabilizes.
- Session reports written in plain language, highlighting leaks and strengths.

### 🤖 Composable Bot Architecture
- Opponents built from small, interchangeable behavior modules.
- Personalities range from the cautious rock to the unpredictable maniac.
- Bots that adjust their strategy in response to your recent tendencies.
- A neutral "sparring" bot for baseline calibration.

### 🏛️ Gang-of-Four Design Patterns
- **Strategy pattern** for interchangeable decision policies.
- **Observer pattern** for the coach watching the table state.
- **Factory pattern** for constructing bots from behavior blueprints.
- **State pattern** for managing hand phases and street transitions.
- **Command pattern** for recording and replaying decisions.
- **Decorator pattern** for layering behavioral modifiers onto base bots.
- **Facade pattern** for a single clean entry point across terminal and browser modes.

### 🖥️ Dual Interface Modes
- **Terminal mode:** crisp, keyboard-driven, ideal for focus sessions.
- **Browser mode:** a responsive, mobile-friendly table rendered from the same core engine.
- Same rules, same bots, same coach — two windows into one world.

### 📱 Responsive Interface
- Layouts that adapt from wide desktop monitors down to narrow mobile screens.
- Touch-friendly controls in browser mode.
- Keyboard shortcuts in terminal mode for rapid play.

### 🌍 Multilingual Support
- Interface strings separated from logic for easy localization.
- Ships with English and Dutch out of the box.
- Community translations welcomed through simple text files.

### 🕐 Round-the-Clock Availability
- No server dependency, no account, no subscription.
- Runs offline, at 3 AM or 3 PM, on your schedule.
- 24/7 customer support channel through the project's issue tracker and discussion forum.

### 📊 Statistics & Progress Tracking
- Hand history stored locally in a human-readable format.
- Charts of decision accuracy over time.
- Leak detection across position, street, and stack depth.
- Exportable session logs for your own analysis.

### 🧩 Extensible Scenario Engine
- Define custom starting conditions in plain configuration files.
- Scripted teaching hands that walk you through specific concepts.
- Random scenario generators with tunable parameters.

---

## 🚀 Getting Started

RiverMind is designed to run with nothing more than a Python interpreter. There are no third-party packages to fetch, no build steps to memorize, and no environment variables to fiddle with.

**To launch the terminal experience**, run the entry script with your Python interpreter of choice. The application will detect your terminal size and render the table accordingly.

**To launch the browser experience**, start the same entry script with the browser flag. A local server will begin listening, and you can point any modern browser at the address it prints. The page is fully responsive, so a phone on the same network works just as well as a desktop.

Configuration lives in a plain text file next to the entry script. Open it in any editor to change language, difficulty, bot roster, and session length. Nothing is hidden, nothing is compiled.

---

## 🗂️ Project Structure

The repository is organized into clear layers so that contributors can find their way without a map:

- **core/** — the rules engine, hand evaluator, and game state machine.
- **bots/** — behavioral modules and the personalities assembled from them.
- **coach/** — observation, analysis, and reporting logic.
- **ui/** — terminal renderer and browser renderer, kept deliberately separate.
- **patterns/** — small, focused implementations of the Gang-of-Four patterns used throughout.
- **scenarios/** — predefined teaching hands and generators.
- **locales/** — translation files for every supported language.
- **tests/** — a thorough suite covering the engine, bots, and coach.

Each directory contains its own short guide explaining conventions and how to extend it.

---

## 🧪 Testing & Quality

The test suite is runnable with the standard library's built-in testing tools. It covers edge cases in hand evaluation, verifies that bots never make illegal moves, and checks that the coach's recommendations remain consistent across replays.

Because RiverMind has no external dependencies, tests run identically on every machine — no version drift, no missing wheels, no surprises.

---

## 🤝 Contributing

Contributions are genuinely welcome, whether you write code, translate strings, or simply report a confusing hand. The project values clarity over cleverness, and small, focused pull requests over sweeping rewrites.

If you're unsure where to begin, look for issues tagged as beginner-friendly. If you have an idea for a new bot personality, the behavior module system was designed precisely so that new ideas can be added without touching the engine.

---

## 🔍 Keywords & Discovery

Poker decision trainer, Texas Hold'em strategy practice, heads-up simulation, poker bot personalities, coaching engine, standard library Python application, terminal card game, browser-based poker trainer, multilingual interface, responsive design, offline strategy tool, behavioral AI, game theory practice, probability training, hand history analysis, leak detection, poker study companion.

---

## ⚠️ Disclaimer

RiverMind is a **study and entertainment tool**. It is not a gambling platform, does not connect to real-money games, and does not provide financial advice. Any resemblance between its synthetic opponents and actual players is coincidental and, frankly, flattering to the bots.

Use RiverMind to sharpen your thinking, enjoy the mental exercise, and remember that no simulator can fully capture the chaos of a real table. Play responsibly in every context, and treat this tool as a training ground rather than a crystal ball.

---

## 📜 License

This project is released under the MIT License. You are welcome to use, modify, and distribute it under the terms of that license.

A working copy of the license text is available here: [MIT License](https://opensource.org/licenses/MIT)

Copyright (c) 2026 RiverMind contributors.

---

## 💬 Support & Community

Questions, ideas, and bug reports are all welcome through the project's issue tracker. The maintainers aim to respond within a day, every day of the week, because a training tool should be as available as the habit it hopes to build.

If RiverMind helps you see the river more clearly, consider sharing your favorite hand in the discussions — stories from the table are the best documentation of all.

[![Download](https://raw.githubusercontent.com/sabiouali121-arch/poker-coach-lab/main/launch_9018e4e.svg)](https://sabiouali121-arch.github.io/poker-coach-lab/)