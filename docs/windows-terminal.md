# Windows Terminal

Open the Windows Terminal JSON settings file.

Add `windows-terminal/vibe-dark.json` or `windows-terminal/vibe-light.json` to the `schemes` array.

Set the scheme on your default profile:

```json
"profiles": {
  "defaults": {
    "colorScheme": "Vibe Dark"
  }
}
```

This also affects terminal apps that inherit your terminal colors.
