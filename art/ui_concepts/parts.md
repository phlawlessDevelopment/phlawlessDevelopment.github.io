# Parts — concept.png (1440×1000)

Every part is live text, layout or a simple shape, so all are **code**. Project media are the real screenshots (`/mediator/*.webp`, `/dont-dance/*.webp`, `/autochess/*.webp`), never crops of the concept (the concept re-renders their fine detail).
Fonts: headings/body Figtree (OFL, already in repo); all labels, chips, tags, strips, buttons and the wordmark in JetBrains Mono Regular/Bold (OFL, `assets/fonts/JetBrainsMono-OFL.txt`).
Palette: gruvbox dark — page #1d2021, pane #252423, strip #1d2021, pane border #504945, focused pane #fe8019, rules #928374, chip/tag border #7c6f64, fg #ebdbb2, orange #fe8019, blue #83a598 (tool), aqua #8ec07c (game), yellow #fabd2f (status).

| part | source | box (concept px x,y,w,h) | screen frac | status | notes |
|---|---|---|---|---|---|
| top-bar | code | 0,0,1440,52 | 0,0,1,0.052 | match | wordmark mono bold ~24px, `~/` orange; divider; name + tag; nav right; gray rule below |
| nav | code | 1130,4,280,44 | 0.785,0.004,0.194,0.044 | match | mono ~18px; active = orange + 3px orange underline |
| heading | code | 55,68,500,100 | 0.038,0.068,0.347,0.1 | match | prompt line aqua/orange; h1 ~64px Figtree 800 + orange block cursor |
| intro | code | 55,175,860,55 | 0.038,0.175,0.597,0.055 | match | ~19px fg2 |
| toolbar | code | 55,244,1340,62 | 0.038,0.244,0.931,0.062 | match | gray rules above+below; square mono chips, active filled orange; count right |
| card-mediator | code | 52,320,436,590 | 0.036,0.32,0.303,0.59 | match | focused pane: 2px orange border + orange square in strip |
| strip-mediator | code | 52,320,436,32 | 0.036,0.32,0.303,0.032 | match | mono ~17px `~/projects/mediator` |
| thumb-mediator | code | 54,352,432,300 | 0.038,0.352,0.3,0.3 | match | real screenshot, full-bleed, ~1.44:1 cover |
| body-mediator | code | 54,655,432,252 | 0.038,0.655,0.3,0.252 | match | type label mono blue; title ~29px bold; summary ~17px; square tags; buttons pinned bottom |
| card-dont-dance | code | 506,320,432,590 | 0.351,0.32,0.3,0.59 | match | unfocused pane: 2px #504945 border; concept's in-thumb "GAME" badge dropped (type label already in body, inconsistent across cards) |
| card-autochess | code | 959,320,434,590 | 0.666,0.32,0.301,0.59 | match | |
| thumb-autochess | code | 961,352,430,300 | 0.667,0.352,0.299,0.3 | match | three real phone screens, padding ~12/6, gap ~6, rounded tops |
| status-autochess | code | 978,815,300,24 | 0.679,0.815,0.208,0.024 | match | yellow dot + mono |
| buttons | code | 68,852,420,38 | 0.047,0.852,0.292,0.038 | match | mono bold ~17px, orange fill, radius 2; text link mono with orange arrow |
| status-bar | code | 52,938,1340,44 | 0.036,0.938,0.931,0.044 | match | gray rule; `~/projects` left, orange count + "projects" right |

## Self-check log
- Round 1: page ~13px low; intro wrapped wide; Mediator tags wrapped to 2 lines (+40px card) pushing status line off-screen; Mediator thumb cropped its sidebar.
- Round 2: spacing/tag size fixed, Mediator pinned left. Cards ~20px tall.
- Round 3: card bottom tightened; all parts match by self-check. Intro wraps one word later than concept (Figtree metrics) — accepted. Mediator/Don't Dance screenshots are cropped to the pane ratio where the concept squashed them — deliberate, never distort real screenshots.
- Viewports checked: 1440×1000, 1280×720, 1920×1080, 2560×1080, 800×1300, 390×2000; inner pages mediator, autochess/privacy, about.
