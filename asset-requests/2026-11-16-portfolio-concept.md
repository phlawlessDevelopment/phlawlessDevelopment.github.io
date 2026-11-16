# Asset request: portfolio homepage UI concept

Project root: /home/phlawless/dev/phlawlessDevelopment.github.io
Engine / consumer: static HTML/CSS website (GitHub Pages). The concept is a design target only; it is rebuilt in HTML/CSS and compared against at 1440×1000.
Art direction: gruvbox dark with orange highlights, terminal / tiling-window-manager flavour, crisp and confident, personal developer portfolio for "Phlawless Development" (Louis Hopkins, software & games). Should feel much more characterful than the baseline, which reads as plain/generic.
Style references (attach as reference images):
- /home/phlawless/dev/phlawlessDevelopment.github.io/art/ui_concepts/baseline.png — current build. Edit/redesign ON TOP of this: same content, same 3 projects, same real screenshots, grid of project cards.
- Real project screenshots to keep inside the cards unchanged: /home/phlawless/dev/phlawlessDevelopment.github.io/mediator/conversation-dark.webp, /home/phlawless/dev/phlawlessDevelopment.github.io/dont-dance/character-select.webp, /home/phlawless/dev/phlawlessDevelopment.github.io/autochess/home.webp, /home/phlawless/dev/phlawlessDevelopment.github.io/autochess/board.webp, /home/phlawless/dev/phlawlessDevelopment.github.io/autochess/roster.webp
Pixel art: no

## Assets

### [x] concept
- Delivery: `art/ui_concepts/concept.png` — 1440×1000, RGB, opaque; normalized with PIL without cropping the header or cards. Issue: screenshot fine details are AI-rendered; the coordinator must use the original unchanged WebP files in the HTML/CSS build.
- Progress: generated with the built-in image_gen tool, visually checked, and PNG dimensions/mode verified. Exact final prompt: `art/ui_concepts/prompt.md`.
- Generation source: `/home/phlawless/.codex/generated_images/01a1e475-7845-78f0-88d1-f0fd58e8a655/exec-6065fcd6-85a8-4304-aba3-ac124f9b8159.png` (1487×1058, RGB); copied and proportionally fitted to the final canvas. The tool accepts five reference paths, so Autochess home was supplied within the baseline; the other four project screenshots were attached individually.
- Path: art/ui_concepts/concept.png  (and write the exact final prompt you used to art/ui_concepts/prompt.md)
- Placeholder at path: no
- Size: 1440×1000 px final (generate landscape, then resize/crop with PIL to exactly 1440×1000; keep the whole page composition — do not crop off the header or the cards), background: opaque
- Content: flat full-page desktop capture of the redesigned homepage, no browser chrome, no device, no perspective. Must contain, with this exact text:
  - Top bar: wordmark "Phlawless Development"; "Louis Hopkins" "Software & games."; nav "Work" (active, orange), "About", "GitHub".
  - Intro: heading "Stuff I've made"; paragraph "I'm Louis. I make games and tools, these days mostly with coding agents. You can try two of these in your browser right now, and the autochess game is in closed testing on Google Play."
  - Filter chips "all 3", "games 2", "tools 1" and a count "3 projects".
  - A grid of three project cards (one row at this width), each with its real screenshot on top, type label, title, one-line summary, tech tags and actions:
    - Mediator — tool — "A group chat with an AI that steps in when people start getting heated." — Java, Spring Boot, WebSocket, SQLite — buttons "Try the demo", "How it works"
    - Don't Dance — game — "One tired monster, too many tiny singers. A wee arcade game, solo or local co-op." — Godot, Local co-op, Browser — "Play in browser", "About the game"
    - Phlawless Autochess — game — "Autochess for your phone, a bit like TFT, played in portrait with one thumb." — Godot, GDScript, Android — status "Closed testing on Google Play" — "Have a look"
  - Ideas welcome (pick a coherent set, don't use all): cards styled as tiling-WM / terminal panes with a title strip (e.g. "~/projects/mediator"), orange focused-window border on one card, monospace labels, subtle gruvbox colour accents per type (aqua games, blue tools), a terminal-prompt line above the heading, small keycap or status-line details, a bottom status bar. Must stay buildable in HTML/CSS: no painted textures, no 3D, no glassmorphism, no gradient blobs, no mascots outside the screenshots, no invented projects, metrics or testimonials.
  - Project screenshots stay recognisable and uncoloured by the theme.
- Used by: index.html + assets/site.css (rebuilt to match)

## Rules for the asset agent
- Use the built-in image_gen tool through $imagegen. Don't use the CLI fallback unless the user asks.
- Copy the final image from $CODEX_HOME/generated_images/... to its exact Path.
  Never overwrite any other existing file (write a sibling `-v2` instead).
- Normalize to the exact Size with PIL. Check the file (dimensions, mode) before you finish.
- Only touch the asset paths, prompt.md and this file. Don't edit site code. The coordinator wires it up.
- Tick each `[ ]` to `[x]` and add a one-line note (final path, size, anything off).
- Start no subagents.
- Final reply: one line per asset, `<asset-id> → <path> (<W×H>, <mode>) ok|issue: …`.
