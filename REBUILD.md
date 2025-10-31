You are a senior full-stack designer-developer and brand stylist.

GOAL
Rebuild my site (currently at https://ontographers-book.vercel.app) using the visual system, structure, and polish of the GitHub repo “cojovi/Ontographer-book” (a fork of Reactive Resume). Keep everything dark-mode by default with a dark-humor edge (Tim Burton / dark fantasy vibes with neon “aurora” accents). Replace all placeholder content with on-brand text derived from my book draft (attached) and invent tasteful filler where needed.

PRIMARY INPUTS
- Current live site content/IA: use only as a reference for minimal sections that exist.  
- Style reference: https://github.com/cojovi/Ontographer-book → borrow its design language: Tailwind tokens, spacing scale, card/tile patterns, timelines/sections, rounded corners, soft shadows, and template-like page rhythm. Do NOT copy its product copy; copy the aesthetic and component feel.
- Book draft (PDF excerpt): mine for titles, blurbs, quotes, and themes. Chapters to surface as section anchors:
  • “Prologue – The Ontographer’s Prelude to Pandemonium”
  • “The Birth of Bedlam”
  • “Adolescence and Anarchy”
  • “College: A Carnival of Chaos”
  • “The Maze of Melancholy”
  • “Philosophies of Foolishness”
  • “The Path to Personal Enlightenment”
  • “Trials of Triumph and Tribulation”
Use these to generate real copy in a witty, introspective, darkly comedic voice.

TECH & ARCHITECTURE
- Next.js (App Router) + TypeScript + TailwindCSS.
- UI kit: compose from Tailwind primitives (inspired by Reactive Resume spacing/typography); optionally use Framer Motion for micro-anims.
- Folder shape:
  /app
    /layout.tsx
    /page.tsx                (Home)
    /chapters/[slug]/page.tsx (Chapter detail pages)
    /about/page.tsx
    /gallery/page.tsx
    /buy/page.tsx
  /components (Hero, Section, Card, Quote, Marquee, TOC, CTA, Footer, Nav, ChapterCard, ReviewCard, AnimatedCover)
  /content (JSON/MD for chapters, reviews, quotes, FAQs)
  /public (og images, cover loops, favicons)

VISUAL SYSTEM
- Palette: near-black canvas (#0b0f1a to #0e0e12), text-gray-200/300, neon accents (aurora vibes: cyan/teal/magenta/purple/acid-lime). Use subtle grain/noise layer. 
- Typography: tall condensed display for headlines (e.g., Oswald/Anton/Unbounded) + humanist mono or grotesk for body (e.g., Inter/Space Mono). 
- Motifs: thin borders, glassy cards, soft glows, neon underlines, starfield/film-grain, “stop-motion jitter” hover micro-motion.
- Components to mirror from the style repo: sectioned layouts with generous negative space, template-like “panels,” pill badges, timeline/chunked content, grid galleries.

PAGES & CONTENT (WRITE THE COPY)
1) Home (single scroll)
   - Hero: Title “An Ontographer’s Tangled Web of Tom Foolery” + punchy logline (10–16 words).
   - Animated cover loop (subtle parallax/shadow flicker).
   - 3 CTA buttons: Read Excerpt • View Chapters • Pre-Order
   - Pull-quotes carousel (3–5 lines) sourced from draft; keep dark wit.
   - “Why Read” three-up: Chaos • Catharsis • Comedy (short bullets).
2) Chapters (index)
   - Grid of chapter cards with moody thumbnails; each card has a 1-sentence hook and a 20–30 word teaser pulled/adapted from the draft.
3) Chapter Detail
   - Banner with neon accent line; 250–400 words excerpt; “Themes” chips (e.g., resilience, self-sabotage, glow-up, jail epiphany, tech-solitude).
   - Pull-quote block and “Continue → Buy” CTA.
4) About the Author
   - Brief bio (Texas roots, paradox-of-persona tone), “Ontographer” definition riff, timeline tile row.
5) Gallery
   - 6–9 images/loops in the abstract/gothic/aurora style. Provide ALT text with dark humor.
6) Reviews/Blurbs
   - Replace placeholders with either real blurbs (if supplied) or witty stylized “mag” blurbs that sound legit without faking endorsements.
7) Buy/Pre-Order
   - Buttons for current store(s) or “Join the list” email capture (store in simple JSON or form backend).
8) Footer
   - Minimal links + social.

DARK HUMOR & TONE (GENERATE THIS)
- Use first-person rumination with sardonic asides. Blend melancholy with mischief.
- Sample micro-copy to produce (generate 3–5 options each):
  • Site tagline
  • 8 chapter one-liners
  • 6 pull quotes (≤ 20 words)
  • About-blurb (80–120 words)
  • 5 FAQ Q/A (funny but useful)

ANIMATION
- Framer Motion for:
  • Hero title letter-fade/kerning wobble (subtle).
  • Card hover: film-grain glow + 2px parallax lift.
  • Section dividers: aurora line sweep.
  • Quote carousel: crossfade with slight jitter for “stop-motion” vibe.

ASSETS TO PRODUCE
- 4 OG images (1200×630): Hero, Chapters, Gallery, Buy.
- Favicon set + maskable PWA icon.
- 2 short MP4/WebM loops for cover animation (no audio, ≤2MB).

SEO & META
- Title/description; canonical; robots; sitemap.
- JSON-LD Book schema (author, name, genre, workExample for excerpts).
- OpenGraph + Twitter cards for every top route.

A11Y & PERF
- 4.5:1 contrast minimum; focus rings; reduced-motion respect.
- Preload fonts; next/image; lazy load non-critical media; Lighthouse ≥ 95.

DELIVERABLES
1) Tailwind theme tokens (colors, radii, shadows) and example classes.
2) Components in /components with example usage.
3) Populated /content JSON/MD (chapters, quotes, reviews) derived from the draft—write the actual text (don’t leave placeholders).
4) A complete /app implementation with working routes.
5) 4 OG images + 2 hero loop assets (placeholder if needed but styled).
6) README with run/build/deploy steps (Vercel).

LICENSE & CREDIT
- Keep MIT attributions where applicable; this is a re-skin inspired by Reactive Resume’s styling patterns, not a literal product clone.

NOW DO IT
- Generate the code, content text, Tailwind config, and assets list in one output. Where images are needed, return detailed prompts for my image tool with the exact style (dark fantasy, aurora neon, Tim-Burton-adjacent, expressive elongated characters). Keep copy tight, punchy, and darkly funny.