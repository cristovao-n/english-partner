# english-assistant

Type an English word and get a detailed explanation: Portuguese translation, meanings by part of speech, usage examples, and synonyms. Every explanation is also appended to `history.md`.

It uses [Claude Code](https://claude.com/claude-code) in headless mode (`claude -p`) as the engine, so it needs no API key or Python dependencies.

## Requirements

- Claude Code installed and logged in (`claude` on your `PATH`)
- Optional: [glow](https://github.com/charmbracelet/glow) to render the output as formatted markdown

## Usage

```sh
./word grasp
./word give up
./word          # prompts for the word
```

To use it from any directory:

```sh
ln -s "$PWD/word" ~/.local/bin/word
```

The history is always written to `history.md` next to the script.

## Customizing

Edit `prompt.md` to change the output format. To change the model, edit `--model` in `word`.
