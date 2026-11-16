Use case: ui-mockup
Asset type: high-fidelity portfolio homepage design target, rebuilt later in static HTML/CSS.
Primary request: Redesign the attached baseline homepage ON TOP OF its existing content and three-project card grid. Make it distinctly characterful, crisp and confident: gruvbox dark, orange highlights, a personal developer's terminal / tiling-window-manager aesthetic. Produce a flat full-page desktop website capture, opaque background, landscape composition at 1440 x 1000 proportions. No browser chrome, no device, no perspective. Keep the entire header, all three cards, all actions and bottom edge visible.

Input images:
Image 1 = baseline.png, edit target and source of the exact page content and three-column layout.
Image 2 = mediator/conversation-dark.webp, supporting insert for the Mediator card. Preserve this real screenshot's contents and original colours.
Image 3 = dont-dance/character-select.webp, supporting insert for the Don't Dance card. Preserve this real screenshot's contents and original colours.
Image 4 = autochess/board.webp and Image 5 = autochess/roster.webp: supporting inserts for the Phlawless Autochess card. The original autochess/home.webp is already visible as the LEFT portrait screenshot inside the Autochess card of Image 1; retain and use that exact existing screenshot too. Show those three portrait screenshots side by side, as in the baseline, with their original imagery and colours. They are flat screenshots, not phone mockups.

Composition and styling:
A polished, buildable web interface with generous 48px outer margins and clear alignment. Warm near-black background #1d2021 / #282828, cream #ebdbb2 headings, muted warm body text #bdae93, orange #fe8019 focus and primary actions, blue #83a598 tool labels, aqua #8ec07c game labels, fine #504945 borders. Flat solid fills only, square or barely rounded corners. Clean bold sans-serif for the large heading and project titles; a legible developer monospace for the wordmark, terminal line, chips, title strips, tech tags and status details. Crisp text and rules, not a painted illustration.

Top bar: horizontal, roughly 78px high, fine bottom border. Left wordmark with a small orange terminal prompt mark; the exact wordmark is "Phlawless Development". Beside it, separated by a thin rule, show "Louis Hopkins" and "Software & games.". Right nav: "Work" active in orange with a short underline, then "About", then "GitHub".

Intro: small terminal-prompt line "~/projects $ ls" above a bold, large, cream heading, approximately 72px, "Stuff I've made". An orange cursor detail is allowed. Under it place the following paragraph, comfortably readable and wrapped across two or three lines, verbatim:
"I'm Louis. I make games and tools, these days mostly with coding agents. You can try two of these in your browser right now, and the autochess game is in closed testing on Google Play."

Below the intro, a compact horizontal filter/status row between fine rules. Filter chips exactly "all 3", "games 2", "tools 1". Make "all 3" selected in orange. Right-aligned count "3 projects".

Main content: exactly THREE equal-width project cards in ONE row, in this order: Mediator, Don't Dance, Phlawless Autochess. Approximately 432px wide with 24px gutters. Cards styled as restrained tiling-WM panes: narrow monospace title strip at the very top, real screenshot region directly below, then type label, title, short summary, tech tags and aligned actions. One orange focused-window outline around Mediator; other panes use fine muted borders. A small orange focus square is allowed in its strip. Use title strips "~/projects/mediator", "~/projects/dont-dance", "~/projects/autochess". Give every card the same image-region height, around 230px, and enough space for ALL text and actions below. Render screenshots unchanged, recognisable, proportional, without recolouring or reillustrating them. Do not apply the gruvbox palette inside project screenshots. Fit the three portrait Autochess screenshots together inside its region, preserving their portrait proportions and as much of each screenshot as possible. Keep all actions visible and at a shared bottom alignment.

Card 1, exact text:
type label "tool" in muted gruvbox blue
title "Mediator"
summary "A group chat with an AI that steps in when people start getting heated."
tech tags "Java", "Spring Boot", "WebSocket", "SQLite"
orange primary button "Try the demo"
secondary action "How it works"

Card 2, exact text:
type label "game" in muted gruvbox aqua
title "Don't Dance"
summary "One tired monster, too many tiny singers. A wee arcade game, solo or local co-op."
tech tags "Godot", "Local co-op", "Browser"
orange primary button "Play in browser"
secondary action "About the game"

Card 3, exact text:
type label "game" in muted gruvbox aqua
title "Phlawless Autochess"
summary "Autochess for your phone, a bit like TFT, played in portrait with one thumb."
tech tags "Godot", "GDScript", "Android"
small status with a yellow dot "Closed testing on Google Play"
orange primary button "Have a look"

The summaries are one short sentence each and may wrap naturally to fit the equal-width cards. Use readable 15-16px body text and about 22px project titles. Use a restrained bottom status bar, thin border, with existing content only: "~/projects" and "3 projects". Let the card grid dominate the lower half; avoid large empty wasted areas. No additional marketing copy.

Invariants: SAME content, SAME three projects, SAME five real screenshots as the references. All exact quoted text must be legible, complete and spelled verbatim. Phlawless is spelled P-h-l-a-w-l-e-s-s. Keep every header and all card bottoms within the full composition. This is a website concept achievable with HTML/CSS borders, spacing, typography and screenshots.
Avoid: invented projects, invented metrics, testimonials, extra slogans, decorative mascots outside the supplied screenshots, pixel-art UI, painted textures, 3D, glassmorphism, gradients, gradient blobs, soft glow, heavy shadows, floating perspective panels, browser window chrome, device frames, watermarks.
