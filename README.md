# Space Up – French & English

A lightweight browser game inspired by the classic "Heads Up" party activity.  The app displays bilingual vocabulary cards with matching emoji artwork so players can practice French and English while playing hands-free on a mobile device.

## Features

- Randomised deck of bilingual vocabulary cards with simple emoji illustrations.
- Device-orientation controls: tilt down for a correct guess, tilt up to pass.
- Gentle motion filtering that requires holding the device briefly to avoid accidental triggers.
- Audio chimes that confirm correct guesses and passes.
- Automatic score keeping with persistent high score storage in `localStorage`.

## Getting Started

Open `index.html` in a mobile browser that supports the DeviceOrientation API.  Tap **Start Game** and hold the phone against your forehead so friends can see the clue.  Tilt the device down and hold for a moment after a correct answer to advance to the next card, or tilt up to skip.

## Development

The project is a single static HTML file with inline CSS and JavaScript.  Images are embedded as data URIs to keep the experience self-contained.  Adjust vocabulary or add new artwork by editing the `icons` object inside `index.html`.

When modifying motion handling logic, test on multiple devices to balance responsiveness with stability.  Audio playback is powered by the Web Audio API and is initialised after the user presses the start button.
