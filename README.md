# Vibe Theme

A minimal monochrome theme set.

![Vibe Dark](assets/hero-dark.png)

![Vibe Light](assets/hero-light.png)

Syntax stays grayscale. Diffs, errors, warnings, and git states keep their color.

This repo ships a few ready-to-use ports and a shared palette for making more.

Terminal tools that inherit terminal colors will pick up the terminal scheme. Tools with their own theme selector need their own native port.

## Prompt

```text
Install Vibe Theme from https://github.com/jasprcodess/vibe-theme across my setup. Use native ports where they exist, use the terminal scheme for terminal-based tools, and create matching ports from palette.json for any vibecoding tools that support custom themes. Default to Vibe Dark unless I already use light themes.
```

## Install

### OpenCode

```bash
mkdir -p ~/.config/opencode/themes
cp opencode/vibe-dark.json opencode/vibe-light.json ~/.config/opencode/themes/
```

Then run `/theme` and choose `vibe-dark` or `vibe-light`.

### Windows Terminal

Open the JSON settings file from Windows Terminal and add `windows-terminal/vibe-dark.json` or `windows-terminal/vibe-light.json` to the `schemes` array.

Set it as the default scheme:

```json
"profiles": {
  "defaults": {
    "colorScheme": "Vibe Dark"
  }
}
```

### VS Code

From `vscode/`:

```bash
npx @vscode/vsce package
code --install-extension vibe-theme-1.0.0.vsix
```

Then open the theme picker and choose `Vibe Dark` or `Vibe Light`.

### Codex

```bash
mkdir -p ~/.codex/themes
cp codex/vibe-dark.tmTheme ~/.codex/themes/
```

Then open Codex and run `/theme`, or set `theme = "vibe-dark"` in `~/.codex/config.toml`.

Docs:

- [OpenCode](docs/opencode.md)
- [VS Code](docs/vscode.md)
- [Windows Terminal](docs/windows-terminal.md)
- [Codex](docs/codex.md)

Palette and rules:

- [palette.json](palette.json)

## License

MIT
