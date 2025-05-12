# Windows-System-Optimizer
A user-friendly Electron app to boost Windows performance by adjusting power plans, visual effects, DPI scaling, and cleaning temporary files — all with a modern UI including progress feedback and cleared-size reporting.

## Features

- **High Performance Power Plan**: Switch to Windows' High Performance mode.
- **Disable Animations & Effects**: Turn off unnecessary UI animations.
- **Reduce Graphics Quality**: Reset DPI scaling to 100%.
- **Clean Temporary Files**: Measure, delete, and report MB cleared in real time.
- **Modern Feedback**: Progress bar, success tick, and cleared-size display.

## Installation

1. Clone or download the repository:
   ```bash
   git clone https://github.com/<your-username>/windows-system-optimizer.git
   ```
2. Change directory:
   ```bash
   cd windows-system-optimizer
   ```
3. Install dependencies:
   ```bash
   npm install
   ```

## Usage

- Launch the app in development:
  ```bash
  npm start
  ```
- Package for Windows (x64):
  ```bash
  npm run package
  ```
  The installer will be in the `dist/` folder.

## Files Overview
- `main.js`: Bootstraps Electron window and handles PowerShell commands.
- `preload.js`: Exposes a secure IPC API to the renderer.
- `index.html`: Main UI layout and styles.
- `renderer.js`: UI logic for button events, progress, and results.
- `package.json`: Project metadata and scripts.

## Contributing

1. Fork the repo.
2. Create a feature branch: `git checkout -b feature-name`.
3. Commit your changes: `git commit -m "Add new feature"`.
4. Push to the branch: `git push origin feature-name`.
5. Open a Pull Request.
