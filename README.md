# Vibe Theme

Monochrome theme for vibecoders. Syntax is grayscale. Diffs, errors, and warnings get color.

Works with OpenCode, VS Code, and Windows Terminal.

## Quick install

Paste this into your AI coding agent:

```
Install the Vibe Theme from https://github.com/jasprcodess/vibe-theme on everything I use.
```

## OpenCode

```bash
mkdir -p ~/.config/opencode/themes
cp opencode/vibe-dark.json opencode/vibe-light.json ~/.config/opencode/themes/
```

Run `/theme` and pick `vibe-dark` or `vibe-light`.

## Windows Terminal

Open settings JSON (`Ctrl+,` > Open JSON file). Add the contents of `windows-terminal/vibe-dark.json` to the `schemes` array. Then set it:

```json
"profiles": {
  "defaults": {
    "colorScheme": "Vibe Dark"
  }
}
```

Any terminal tool (Claude Code, Codex, etc.) inherits these colors automatically.

## VS Code

Install from the [VS Code Marketplace](https://marketplace.visualstudio.com/) (coming soon), or manually:

```bash
cd vscode
npx @vscode/vsce package
code --install-extension vibe-theme-1.0.0.vsix
```

Then `Ctrl+K Ctrl+T` and pick "Vibe Dark" or "Vibe Light".

## License

MIT
