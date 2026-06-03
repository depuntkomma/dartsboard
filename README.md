# Precision Touch Dart Board

A web-based darts scoreboard application designed for touch devices, providing a seamless and professional scoring experience for two-player darts matches.

## Features

- **Game Modes:** Support for 101, 301, and 501 game targets.
- **Match Rules:** Choose between:
  - **Double In / Double Out (DI/DO):** Must start and end with a double.
  - **Double Out Only (DO):** Open scoring, but must end with a double.
  - **No Doubles (Straight Open):** Open scoring and open ending.
- **Interactive SVG Dartboard:** A high-quality, interactive dartboard for precise score input.
- **Touch-Optimized Viewport:** Supports panning and zooming for easier navigation on mobile devices.
- **Real-time Scoring:** Automatic score calculation, turn tracking (3 darts per turn), and bust logic.
- **Checkout Suggestions:** Displays professional checkout routes (e.g., T20, T20, D16) when a player reaches a finishable score.
- **Voice Feedback:** Integrated speech synthesis to call out scores, busts, and the winner of the leg, with a selection menu to choose from all available system voices.
- **Game Controls:**
  - **Undo:** Revert the last dart thrown.
  - **Miss:** Register a missed dart.
  - **Reset:** Quickly start a new game or change modes.
  - **Voice:** Open a menu to select the preferred referee voice.

## Tech Stack

- **HTML5:** Semantic structure and SVG for the dartboard.
- **CSS3:** Responsive layout using Flexbox and CSS variables, with a dark-themed professional aesthetic.
- **JavaScript (Vanilla):** Core game engine, state management, and interaction logic. No external dependencies.

## UI Structure

- **Setup Wizard:** A sequential modal overlay for selecting game mode and rules.
- **Top HUD:** Displays player names, current scores, status badges (e.g., "Need Double In"), and checkout suggestions.
- **Middle Viewport:** Houses the interactive SVG dartboard with pan/zoom capabilities.
- **Bottom HUD:** Shows turn status, current rule set, the three dart slots for the current turn, and primary action buttons.

## Getting Started

Simply open `index.html` in any modern web browser. The application is designed to be mobile-friendly and can be added to the home screen on iOS/Android for a fullscreen app experience.

## Usage

1. **Select Mode:** Choose 101, 301, or 501 on startup.
2. **Select Rules:** Pick the match modifiers (DI/DO, DO, or None).
3. **Play:** Tap segments on the dartboard to register hits.
4. **Win:** The first player to reach exactly zero according to the rules wins the leg.
