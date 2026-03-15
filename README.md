# Vibe Theme

Monochrome theme for vibecoders. Syntax is grayscale. Diffs, errors, and warnings get color. Everything else stays quiet.

Works with OpenCode, VS Code, Windows Terminal (which means Claude Code and Codex also get themed), and Codex syntax highlighting.

## Quick install

Paste this into Claude Code, Codex, OpenCode, or any AI coding agent:

```
Install the Vibe Theme from https://github.com/jasprcodess/vibe-theme on everything I use. Clone the repo, then:
- Copy opencode/vibe-dark.json and opencode/vibe-light.json to ~/.config/opencode/themes/
- Copy codex/vibe-dark.tmTheme to ~/.codex/themes/
- Add the Windows Terminal scheme from windows-terminal/vibe-dark.json to my Windows Terminal settings.json schemes array and set it as the default colorScheme
- For VS Code, install the extension from the vscode/ folder using "code --install-extension" after packaging with vsce, or just copy the theme files manually
```

## Manual install

### OpenCode

```bash
mkdir -p ~/.config/opencode/themes
cp opencode/vibe-dark.json opencode/vibe-light.json ~/.config/opencode/themes/
```

Then run `/theme` in OpenCode and pick `vibe-dark` or `vibe-light`.

### Windows Terminal (also themes Claude Code + Codex)

Open your Windows Terminal settings (`Ctrl+,` > Open JSON file) and add the contents of `windows-terminal/vibe-dark.json` (or `vibe-light.json`) to the `schemes` array. Then set it on your profile:

```json
{
  "profiles": {
    "defaults": {
      "colorScheme": "Vibe Dark"
    }
  }
}
```

Claude Code and Codex both inherit terminal colors, so this themes them too.

### Codex syntax highlighting

```bash
mkdir -p ~/.codex/themes
cp codex/vibe-dark.tmTheme ~/.codex/themes/
```

Then run `/theme` in Codex and pick `vibe-dark`.

### VS Code

From the `vscode/` folder:

```bash
cd vscode
npx @vscode/vsce package
code --install-extension vibe-theme-1.0.0.vsix
```

Then open VS Code, `Ctrl+K Ctrl+T`, pick "Vibe Dark" or "Vibe Light".

## What gets color

- Diffs (green = added, red = removed)
- Errors, warnings, success indicators
- Git decorations in the file tree
- Terminal red/green/yellow for commands that use them

## What stays monochrome

- All syntax highlighting (keywords, functions, strings, variables, types, operators)
- UI chrome (backgrounds, borders, tabs, sidebar)
- Markdown rendering

## License

MIT
