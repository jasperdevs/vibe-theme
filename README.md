# Vibe Theme

A minimal theme set for OpenCode, VS Code, and Windows Terminal.

![Vibe Theme Preview](assets/preview.png)

Syntax stays grayscale. Diffs, errors, warnings, and git states keep color.

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

More details:

- [OpenCode](docs/opencode.md)
- [VS Code](docs/vscode.md)
- [Windows Terminal](docs/windows-terminal.md)

## License

MIT
