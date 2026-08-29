# Ghostty Theme Catalog

Two single-file static pages, no build step and no dependencies.

## [Themes](https://ancplua.github.io/ghostty-theme-catalog/) — `index.html`

Searchable catalog of 463 Ghostty themes with live previews. Filter by
name, dark/light, or starred; sort A–Z or by mood; group by family. Each
theme opens a modal with a rendered terminal preview, the full 16-colour
palette, and the config block to paste into `~/.config/ghostty/config`.
Starred themes persist in `localStorage`. Press `?` for shortcuts.

## [Sound Lab](https://ancplua.github.io/ghostty-theme-catalog/sounds.html) — `sounds.html`

Ten notification chimes for "Claude finished working", **synthesized in
the browser** with the Web Audio API — additive inharmonic partials with
per-partial decay, struck as one or more notes and repeated on a timer.
No audio files are shipped or uploaded.

Shape a chime with the sliders (repeats, gap, pitch, decay, peak level),
watch the rendered waveform, then **Download .wav** and install it:

```sh
mv ~/Downloads/claude-<preset>-x<n>.wav ~/.config/ghostty/sounds/claude-done.wav
```

Drag a local audio file onto the page to decode and draw it behind the
synth trace for comparison — it is read with the File API and never
leaves your machine.

The macOS system-tone table lists tone *names* only, with the
`claude-sound set <name> <repeats>` command to build each one locally.
Apple's audio is not redistributed here.
