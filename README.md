# Vibe Theme

Monochrome themes for [OpenCode](https://opencode.ai) built for vibecoding.

Syntax highlighting is grayscale. Diffs, errors, and warnings get color. Everything else stays out of the way.

## Variants

- **vibe-dark** - matte dark gray
- **vibe-light** - soft light gray

## Install

Copy the theme files to your OpenCode themes directory:

```bash
# macOS / Linux
mkdir -p ~/.config/opencode/themes
cp vibe-dark.json vibe-light.json ~/.config/opencode/themes/

# Windows
mkdir "$env:USERPROFILE\.config\opencode\themes" -Force
copy vibe-dark.json, vibe-light.json "$env:USERPROFILE\.config\opencode\themes\"
```

Then run `/theme` in OpenCode and pick `vibe-dark` or `vibe-light`.

## License

MIT
