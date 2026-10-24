# Personal Academic Homepage — Design Memo

**Project:** Personal Academic Homepage  
**Design Theme:** Nostalgia 1990s × Japanese Personal Web  
**Target Platform:** GitHub Pages  
**Implementation:** HTML5 + CSS3, Zero JavaScript  
**Status:** Design Specification v1.0

---

## 1. Project Vision

Create a lightweight, retro-inspired personal academic homepage combining:

- The desktop UI aesthetics of Windows 95/98.
- Japanese personal websites from the late 1990s to early 2000s.
- Traditional Japanese university laboratory homepages.
- The simplicity and independence of the early personal web.

The website should feel like an academic researcher's carefully maintained personal corner of the internet around 1999–2003.

It must remain professional, readable, fast, and easy to maintain.

**Core design philosophy:**

> A personal homepage from the early internet, maintained by a modern computer scientist.

The website should feel hand-crafted rather than generated from a contemporary portfolio template.

### Design Keywords

`Retro Computing` · `Japanese Web` · `Windows 98` · `Academic` · `Vernacular Web` · `Minimalism` · `Pixel UI` · `Handcrafted HTML`

### Visual Priority

1. Academic credibility and readability.
2. Nostalgic identity and personality.
3. Lightweight implementation.
4. Responsive behavior.
5. Decorative details.

Retro aesthetics should never compromise academic usability.

---

## 2. Visual References

### Primary Reference: Nostalgia 1990s

Reference:

https://github.com/luost26/academic-homepage-nostalgia-1990s

Live demo:

https://luost26.github.io/academic-homepage-nostalgia-1990s/

Borrow the following design concepts:

- Classic gray beveled borders.
- Inset white content panels.
- Windows 95/98-inspired colors.
- Compact desktop-style navigation.
- Small pixel icons.
- Traditional UI typography.
- Rectangular interface elements.

Do not reproduce the entire theme.

Avoid the large desktop simulation, overly complex component hierarchy, unnecessary scripts, and excessively wide layouts.

### Secondary Reference: Japanese Personal Web

Draw inspiration from Japanese personal homepages circa 1998–2003.

Important elements:

- `HOME`, `PROFILE`, `RESEARCH`, `LINKS` navigation.
- `What's New` / `更新履歴` sections.
- `Last Updated` timestamps.
- Small `NEW!` labels.
- Simple horizontal rules.
- Plain HTML links.
- Compact side navigation.
- Personal link collections (`リンク集`).
- Small decorative pixel graphics.
- A handcrafted, slightly imperfect appearance.

These details should be subtle and intentional.

### Overall Balance

- 40% traditional Japanese academic homepage.
- 35% Windows 95/98 desktop UI.
- 25% early Japanese personal web.

Avoid excessive decoration, colorful gradients, animated GIFs, and novelty effects.

---

## 3. Layout Specification

### Desktop Layout

Use a centered, fixed-maximum-width site container.

Recommended width: **880px to 960px**.

The page should resemble a traditional early-2000s website rather than a contemporary full-width web application.

Structure:

```text
+------------------------------------------------------+
| PERSONAL WEB PAGE                      [HOME] [MAIL]  |
+------------------------------------------------------+
| Zihang Hu / 胡子航                                    |
| Software Engineering & AI Research                   |
+--------------+---------------------------------------+
| NAVIGATION   |                                       |
|--------------|  Welcome to My Homepage               |
| > Home       |  -------------------------------      |
| > Profile    |                                       |
| > Research   |  Profile / About Me                   |
| > Papers     |                                       |
| > Projects   |  Research Interests                   |
| > Notes      |                                       |
| > Links      |  -------------------------------      |
|              |                                       |
|--------------|  Selected Publications                |
| INFORMATION  |                                       |
|--------------|  What's New                           |
| Last Update  |                                       |
| 2026.10.24   |                                       |
+--------------+---------------------------------------+
| Copyright / Contact / Best viewed with any browser   |
+------------------------------------------------------+
```

### Layout Rules

Use a two-column structure on desktop:

- Sidebar: approximately 170–190px.
- Main content: remaining width.
- Column gap: 12–20px.

Keep all elements aligned to a restrained pixel-like grid.

The sidebar must be functional, not merely decorative.

The site header should not be sticky.

No animated transitions between pages.

### Mobile Layout

On screens below 700px:

- Convert the layout into a single column.
- Move navigation above the main content.
- Arrange navigation links in compact, wrapping rows.
- Remove any unnecessary decorative side panels.
- Keep every page readable without horizontal scrolling.

Do not use JavaScript for responsive behavior.

Use CSS media queries only.

---

## 4. Color System

Use a restrained Windows 98-inspired palette combined with traditional Japanese academic website colors.

| Element | Color | Hex |
|---|---|---|
| Page background | Muted teal | `#4C7776` |
| Outer panel | Classic silver | `#C0C0C0` |
| Main content | Warm white | `#FAFAF7` |
| Header | Deep navy | `#16356B` |
| Header accent | Muted blue | `#3865A0` |
| Body text | Near black | `#222222` |
| Hyperlink | Classic blue | `#0000AA` |
| Visited hyperlink | Muted purple | `#663399` |
| Border highlight | White | `#FFFFFF` |
| Border shadow | Dark gray | `#606060` |
| Minor metadata | Neutral gray | `#666666` |

### Color Rules

The muted teal background is used only outside the main website frame.

Reading surfaces should remain warm white.

Silver should primarily appear in navigation, the frame, headings, and metadata panels.

Avoid modern pastel gradients, translucent cards, glassmorphism, and neon accents.

Subtle two-tone desktop-style gradients are acceptable for the top title bar.

---

## 5. Borders and UI Elements

Use classic Windows 95/98 beveled borders sparingly.

### Raised Panel

A raised panel should have:

- Light top and left edges.
- Dark bottom and right edges.
- Square corners.
- No drop shadows.

### Inset Panel

An inset panel should have:

- Dark top and left edges.
- Light bottom and right edges.
- White or near-white interior.

Use inset panels for main reading surfaces and selected metadata blocks.

### General Rules

- `border-radius: 0`
- No box shadows.
- No glass or transparency effects.
- No floating cards.
- No material-design components.
- No modern pill-shaped buttons.

Buttons should resemble old HTML buttons or simple text links.

Do not make every paragraph or publication a separate box. The page should remain document-oriented rather than dashboard-oriented.

---

## 6. Typography

Typography should combine early desktop interfaces with traditional academic readability.

### Interface Typography

Use system sans-serif fonts:

```css
font-family:
  Tahoma,
  Verdana,
  "MS PGothic",
  "Meiryo",
  sans-serif;
```

Recommended for:

- Navigation.
- Window title bars.
- Section labels.
- Metadata.
- Buttons.

### Academic Content Typography

Use simple, readable fonts:

```css
font-family:
  Georgia,
  "Times New Roman",
  "Yu Mincho",
  serif;
```

Recommended for:

- Research descriptions.
- Biography.
- Publications.
- Long-form notes.

### Monospace Typography

Use monospace for:

- Dates.
- Version labels.
- File names.
- Technical metadata.
- Small footer messages.

### Size Guidance

| Element | Size |
|---|---|
| Site title | 23–26px |
| Main heading | 19–21px |
| Section heading | 15–17px |
| Body text | 15–16px |
| Navigation | 13–14px |
| Metadata | 12–13px |
| Tiny pixel labels | 11–12px |

Use a body line-height between 1.6 and 1.8.

Avoid reproducing historically tiny text sizes throughout the entire site.

---

## 7. Navigation Design

The navigation should resemble a classic Japanese personal website menu.

Example:

```text
[ MENU ]

■ HOME
□ PROFILE
□ RESEARCH
□ PUBLICATIONS
□ PROJECTS
□ NOTES
□ LINKS

----------------

[ INFORMATION ]

Last Updated
2026.10.24

Status: ONLINE
```

### Behavior

- Navigation should use ordinary HTML anchor elements.
- Current page should have a visually distinct active state.
- Hover states should be simple color or underline changes.
- No dropdown menus.
- No hamburger-menu JavaScript.
- No SPA routing.

Use actual pages or valid anchor targets for all links.

Do not create nonfunctional buttons for decoration.

---

## 8. Homepage Content Structure

The homepage should prioritize research identity over decoration.

### 8.1 Welcome

A compact welcome area containing:

- Name: Zihang Hu / 胡子航.
- Current academic affiliation.
- Research identity.
- Email and academic profile links.

Optional profile photo:

- Small rectangular image.
- Approximately 120–150px wide.
- Square corners.
- Thin gray or beveled border.

Avoid oversized hero images and modern profile cards.

### 8.2 About Me

Brief academic biography.

Keep the section simple, approximately one or two paragraphs.

### 8.3 Research Interests

Initial topics:

- Software Engineering.
- Software Testing.
- LLM-based Agents.
- AI for Software Engineering.
- Formal Methods.
- AI Safety and Security.

Prefer a compact bullet list or short paragraphs.

### 8.4 Selected Publications

Display publications as traditional academic bibliography entries.

Each publication may contain:

- Title.
- Authors.
- Venue and year.
- PDF link.
- Code link.
- Project link.

Example:

```text
[2026] Paper Title
       Author A, Author B, Author C
       Conference / Journal
       [PDF] [Code] [BibTeX]
```

Use plain text links instead of modern colored badges.

### 8.5 Projects

A concise list of research and engineering projects.

Each project should have a title, short description, and relevant links.

Do not use large image cards unless an image conveys essential technical information.

### 8.6 What's New / 更新履歴

A small reverse-chronological update list.

Example:

```text
[ WHAT'S NEW? ]

2026.10.24  Website established.       NEW!
2026.10.15  Research notes updated.
2026.09.01  New project added.
```

This is a key Japanese personal-web element.

Dates should use the `YYYY.MM.DD` format.

The `NEW!` label should be static, small, and colored red or orange. Do not use blinking effects.

Never fabricate academic achievements or updates. Placeholder examples must be clearly identified or replaced before publication.

### 8.7 Links / リンク集

Include links to:

- GitHub.
- Google Scholar, when available.
- Academic institution.
- Research collaborators or laboratory.
- Selected personal technical resources.

Links should look like a manually curated personal collection.

---

## 9. Retro Decorative Elements

Use a small number of intentional decorations.

### Recommended

**A. Pixel Icons**

Use 16×16 or 32×32 images.

Possible motifs:

- Computer.
- Floppy disk.
- Document.
- Folder.
- Mail envelope.
- Book.
- Terminal.

Prefer locally hosted PNG or GIF images.

Avoid using emoji as a substitute for pixel graphics.

Preserve native pixel resolution or use integer scaling with `image-rendering: pixelated`.

**B. Classic Section Headers**

Example:

```text
[+] RESEARCH INTERESTS
----------------------------------
```

A small pixel icon may precede the heading.

**C. Last Updated**

Place this in the sidebar or footer.

**D. Web Version Label**

Optional:

```text
PERSONAL HOMEPAGE
VERSION 1.0 / EST. 2026
```

**E. Small Footer Badge**

A custom 88×31-style retro badge is allowed.

It may contain:

```text
HTML + CSS
NO JAVASCRIPT
```

The badge should be static and locally hosted.

### Optional

- Small `Under Construction` marker for genuinely unfinished pages.
- A minimal `Site Map`.
- A tiny retro-style ASCII divider.
- A static, decorative visit counter with clear labeling (never present a fictional value as real traffic).

### Prohibited

- Autoplay MIDI.
- Background music.
- Animated cursor trails.
- Flashing text.
- Scrolling marquees.
- Fake browser window controls.
- Decorative fake error messages.
- Pop-up windows.
- Large collections of unrelated GIFs.
- External visitor-tracking widgets.

The goal is nostalgia, not visual chaos.

---

## 10. Page Architecture

Initial pages:

```text
/
├── index.html
├── profile.html
├── research.html
├── publications.html
├── projects.html
├── notes/
│   └── index.html
├── links.html
└── 404.html
```

All pages should share the same visual structure:

1. Header.
2. Sidebar navigation.
3. Main content.
4. Footer.

Avoid duplicating inconsistent layouts.

The active page should be identifiable in the navigation.

### Notes

The Notes section should support future articles about research, software engineering, programming, and technical experiments.

Long-form notes must prioritize readability over nostalgic decoration.

Provide standard heading hierarchies, code blocks, lists, tables, and citations where necessary.

---

## 11. Technical Constraints

### Strict Requirements

- No JavaScript.
- No React.
- No Vue.
- No Tailwind.
- No Bootstrap.
- No Node.js build pipeline.
- No external analytics.
- No external font CDN.
- No client-side rendering.
- No unnecessary network requests.

Use HTML5 and CSS3 only.

The website must work when JavaScript is disabled.

### Preferred Implementation

```text
/
├── index.html
├── profile.html
├── research.html
├── publications.html
├── projects.html
├── links.html
├── 404.html
├── notes/
│   └── index.html
├── assets/
│   ├── css/
│   │   └── style.css
│   └── images/
│       ├── portrait.webp
│       ├── icons/
│       └── badges/
├── README.md
└── .nojekyll
```

### CSS Architecture

Organize `style.css` into sections:

1. Design tokens.
2. Base typography and resets.
3. Site container.
4. Classic beveled borders.
5. Header.
6. Sidebar.
7. Content.
8. Academic publications.
9. Retro decorations.
10. Mobile layout.
11. Accessibility.
12. Print styles.

Use CSS custom properties for theme colors and dimensions.

### Optional Future Extension

A static-site generator may be introduced later if managing publications and notes manually becomes inconvenient.

Jekyll or Hugo is acceptable only as a build-time tool.

The generated website must remain ordinary static HTML/CSS and should not require browser-side JavaScript.

---

## 12. Accessibility and Performance

The site should retain modern technical quality beneath its retro appearance.

Requirements:

- Semantic HTML5.
- Correct heading hierarchy.
- Keyboard-accessible navigation.
- Visible focus indicators.
- Meaningful link text.
- Sufficient text contrast.
- Responsive mobile layout.
- Images with appropriate alt text.
- No layout overflow at 320px viewport width.
- No animation required for navigation.
- No JavaScript dependency.
- Print-friendly academic content.

Use system fonts whenever possible.

Keep images small and optimized.

Avoid unnecessary third-party resources.

Target:

- Small page size.
- Fast first render.
- Minimal HTTP requests.
- Functional offline when static assets are available locally.
- Good compatibility with Firefox, Chromium, and Safari.

---

## 13. Anti-Patterns

The implementation must NOT resemble:

- A modern SaaS landing page.
- A startup product homepage.
- A Tailwind portfolio template.
- A Material Design dashboard.
- A macOS desktop simulation.
- A terminal-only hacker homepage.
- A cyberpunk website.
- A highly animated personal portfolio.

Specifically avoid:

- Oversized hero sections.
- Full-screen illustrations.
- Giant typography.
- Rounded card grids.
- Glassmorphism.
- Scroll-triggered animation.
- Complex responsive menus.
- Decorative charts.
- Parallax effects.
- Large empty spaces designed only for visual drama.

Avoid excessive visual polishing that eliminates the handcrafted character of early personal websites.

A slight sense of utilitarian imperfection is desirable, but broken alignment and poor usability are not.

---

## 14. Implementation Workflow for Coding Agent

### Phase 1 — Visual Foundation

Implement:

- Site background.
- Centered outer frame.
- Classic beveled border system.
- Header.
- Sidebar.
- Main reading panel.
- Footer.
- Responsive layout.

Use placeholder content initially.

Do not implement complex content functionality before establishing the visual system.

### Phase 2 — Homepage

Implement the academic homepage with:

- Welcome.
- About.
- Research interests.
- Selected publications.
- What's New.
- Contact information.

Ensure the layout reflects the intended nostalgic style rather than modern component libraries.

### Phase 3 — Internal Pages

Implement consistent templates for:

- Profile.
- Research.
- Publications.
- Projects.
- Notes.
- Links.
- 404.

Provide navigation between pages using ordinary hyperlinks.

### Phase 4 — Decorative Refinement

Add a restrained set of retro details:

- Pixel icons.
- Classic heading treatments.
- Small badges.
- Sidebar metadata.
- Updated date.
- Retro footer.

Do not increase visual complexity unnecessarily.

### Phase 5 — Verification

Check:

- Desktop layout at 1440px and 1024px.
- Tablet layout at 768px.
- Mobile layout at 390px and 320px.
- Keyboard navigation.
- Link correctness.
- Text wrapping.
- Academic content readability.
- No browser-side JavaScript.
- No external runtime dependencies.

Inspect the rendered website rather than relying solely on source-code correctness.

The final result should be deployable directly to GitHub Pages.

---

## 15. Acceptance Criteria

The implementation is complete when:

- [ ] The website clearly evokes a 1999–2003 Japanese personal homepage.
- [ ] Windows 95/98-inspired visual elements are recognizable.
- [ ] The appearance remains appropriate for an academic researcher.
- [ ] Publications and research information are easy to find.
- [ ] Desktop navigation uses a compact classic sidebar.
- [ ] Mobile navigation is usable without JavaScript.
- [ ] All pages share consistent visual styling.
- [ ] The website contains no JavaScript or frontend framework.
- [ ] No mandatory external resources are required.
- [ ] All links and navigation paths work.
- [ ] The site can be hosted as static files on GitHub Pages.
- [ ] The implementation remains readable and easy to maintain.

## 16. Final Design Direction

The finished homepage should resemble a personal academic website created by a Japanese computer science researcher in the early 2000s, with a subtle Windows 98 influence.

It should feel modest, technical, slightly nostalgic, and personal.

The main impression should be:

**"An old-fashioned researcher's corner of the web, carefully preserved and still actively maintained."**

Do not optimize for fashionable modern portfolio aesthetics.

Optimize for authenticity, readability, longevity, and personality.
