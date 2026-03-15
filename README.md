# Vibe Theme for OpenCode

A monochrome theme built for vibecoders.

You don't read code line by line. You prompt, review diffs, accept or reject, and move on. Your theme should reflect that.

## Philosophy

- **Syntax is monochrome.** Keywords, functions, variables, strings — all grayscale. The AI wrote it, you don't need rainbow highlighting to parse it.
- **Diffs are colored.** Green for added, red for removed. The only thing that matters when you're reviewing AI output.
- **Errors and warnings stand out.** Red for errors, yellow for warnings, green for success. Things that need your attention get color.
- **Everything else is calm.** Neutral backgrounds, subtle borders, clean text. No distractions.

## Variants

| Theme | Description |
|-------|-------------|
| `vibe-dark` | Dark matte black background. Not pitch black, not depressing. |
| `vibe-light` | Clean light gray background. Easy on the eyes without being stark white. |

## Install

### Option 1: User-wide (all projects)

Copy the theme files to your OpenCode themes directory:

**macOS / Linux:**
```bash
mkdir -p ~/.config/opencode/themes
cp vibe-dark.json vibe-light.json ~/.config/opencode/themes/
```

**Windows:**
```powershell
mkdir -Force "$env:USERPROFILE\.config\opencode\themes"
copy vibe-dark.json, vibe-light.json "$env:USERPROFILE\.config\opencode\themes\"
```

### Option 2: Project-specific

```bash
mkdir -p .opencode/themes
cp vibe-dark.json vibe-light.json .opencode/themes/
```

## Activate

Run `/theme` in OpenCode and select `vibe-dark` or `vibe-light`.

Or set it in your `tui.json`:

```json
{
  "$schema": "https://opencode.ai/tui.json",
  "theme": "vibe-dark"
}
```

## License

MIT
