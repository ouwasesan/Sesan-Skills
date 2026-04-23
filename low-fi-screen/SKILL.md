---
name: low-fi-screen
description: Create low-fidelity website and mobile-app structures for stakeholder review. Use when the user wants a page or screen structure, block layout, wireframe-style content architecture, boxed ASCII flow, or a prompt for Figma Make to visualize a website, landing page, dashboard, or mobile app screen before final UI design.
metadata:
  short-description: Create low-fidelity page and screen structures
---

# Low-Fi Screen

Use this skill to turn a website or page idea into a clear low-fidelity structure before final UI design or copywriting.

## Modes

This skill supports four explicit output modes. Use the mode name in the request when you want a specific deliverable.

### Mode A: Page Wireframe

Use this when the user wants the page itself represented as a low-fidelity structure.

Best for:

- homepage wireframes
- landing page structures
- dashboard screen layouts
- mobile screen layouts
- continuous page ASCII mockups
- simplified visual hierarchy reviews

Default output:

- a page-like ASCII layout
- one continuous composition or a small set of connected blocks
- light content cues inside boxes
- hierarchy, spacing, and page flow first

Prompt cues:

- "Use Mode A"
- "Create a page wireframe"
- "Show the homepage structure"
- "Turn this into a continuous ASCII layout"

### Mode B: Content Architecture Board

Use this when the user wants a strategy artifact for workshop review, stakeholder alignment, or content planning rather than a page-like wireframe.

Best for:

- homepage content architecture boards
- stakeholder review boards
- workshop-ready block maps
- editorial hierarchy reviews
- restructuring existing homepages
- KEEP / ADD / MOVE / REVIEW style outputs

Default output:

- numbered vertical blocks
- each block includes block number, title, purpose, key content, suggested copy, and status label
- looks like a strategic review board, not a UI mockup
- suitable for leadership, strategy, and content-team discussions

Prompt cues:

- "Use Mode B"
- "Create a homepage content architecture board"
- "Show this as numbered blocks"
- "Add KEEP, MOVE, ADD, REVIEW labels"
- "Make it suitable for stakeholder workshop review"

### Mode C: Figma Prompt

Use this when the user wants the structure translated into a prompt for Figma Make or another design-generation workflow.

Best for:

- turning an ASCII structure into a Figma-ready prompt
- converting a board or wireframe into a low-fi design brief
- handing structure to design for visualization

Default output:

- a ready-to-paste Figma Make prompt
- clear style instructions
- explicit section order
- structural guidance, hierarchy, and annotation rules

Prompt cues:

- "Use Mode C"
- "Turn this into a Figma prompt"
- "Convert this wireframe into a Figma Make prompt"
- "Create a low-fi design prompt"

## How To Use

Choose the mode first, then describe the page or paste the source material.

### Quick usage pattern

```text
Use low-fi-screen in Mode A.
Turn this screenshot into a low-fidelity ASCII homepage wireframe.
```

```text
Use low-fi-screen in Mode B.
Turn this homepage idea into a content architecture board with numbered blocks and KEEP / ADD / MOVE labels.
```

```text
Use low-fi-screen in Mode C.
Convert this ASCII structure into a Figma Make prompt for a low-fidelity stakeholder review board.
```

### What to provide

The skill works best when the user provides one or more of these:

- a screenshot
- existing page sections
- approved copy fragments
- section goals
- a competitor reference
- an ASCII wireframe to convert
- a request to restructure an existing homepage

### Recommended phrasing by mode

For Mode A:

```text
Use low-fi-screen in Mode A.
Create a continuous low-fidelity homepage wireframe from this screenshot.
Keep it page-like, not a content board.
```

For Mode B:

```text
Use low-fi-screen in Mode B.
Create a homepage content architecture board, not a UI wireframe.
Show numbered vertical blocks.
Each block should include:
- block number
- block title
- purpose
- key content
- suggested copy
- status label: KEEP, ADD, MOVE, or REVIEW
```

For Mode C:

```text
Use low-fi-screen in Mode C.
Turn this structure into a Figma Make prompt.
Keep it grayscale, presentation-friendly, and suitable for stakeholder review.
```

### Selection rule

If the user does not specify a mode:

- default to Mode A for page or screen structure requests
- default to Mode B when the user wants strategy, workshop, or stakeholder review artifacts
- default to Mode C when the user explicitly asks for Figma, Make, or a design-generation prompt

This skill is for:

- homepage structure
- landing page structure
- feature page structure
- product page structure
- service page structure
- dashboard or portal page structure
- mobile app home screens
- mobile app onboarding flows
- mobile dashboard screens
- tab-based app structures
- settings or profile screens
- support and utility screens in mobile apps
- stakeholder review boards
- workshop-friendly content architecture
- Figma Make prompts for low-fi visualization

This skill is not for polished UI design. It should produce structure first.

## Website Layout With Existing Content

Use this mode when the user already has website content, homepage allocations, section ideas, or approved copy fragments and wants help turning them into a stronger layout.

The job here is not to invent a new content strategy. The job is to:

- show hierarchy through box size and placement
- communicate what matters most before final UI design
- give each section a clear visual role
- include just enough content inside each box to show what belongs there
- help stakeholders see emphasis, sequence, and structure quickly

In this mode:

- use boxes to communicate importance, not just containment
- make the most important content visibly dominant
- keep secondary content supportive and smaller
- show section purpose through a small amount of representative content
- avoid overfilling boxes with detailed copy
- prefer content cues over full copy blocks unless the user asks for more

When the user already has content, structure it like this:

1. Identify the most important content.
2. Give that content the strongest box, placement, or visual prominence.
3. Group related secondary items into supporting cards or modules.
4. Keep utilities and lower-priority items quieter.
5. Use labels, short headlines, CTA placeholders, image areas, and trust cues to show what belongs there.

What this should feel like:

- not empty boxes
- not full copywriting
- not a finished UI
- a layout blueprint with enough content direction to guide design decisions

This is especially useful for:

- website homepage restructuring
- content already allocated to a homepage
- service or product pages with approved content blocks
- stakeholder reviews where layout is the main question
- Figma Make prompts that need both structure and light content cues

## Rhythm Defaults

When suggesting low-fidelity web or mobile structures, use a consistent spacing and corner-radius rhythm by default.

### Spacing rhythm

- Treat `8px` as the main layout rhythm.
- Use `4px` increments for finer alignment and smaller component adjustments.
- Prefer spacing values that map cleanly to a 4px/8px system.
- Use larger gaps as simple multiples of the base rhythm.

Good default spacing choices:

- `4px` for fine alignment
- `8px` for compact spacing
- `12px` for small grouped spacing
- `16px` for regular card/component spacing
- `24px` for section spacing inside dense layouts
- `32px` for major group separation
- `48px`, `64px`, `80px`, `96px`, `128px` for large section rhythm

### Border-radius rhythm

- Use corner radii from a small, consistent token family rather than arbitrary values.
- Prefer these radii for low-fidelity structure:
  - `0px` sharp
  - `4px` subtle rounding
  - `8px` standard rounded UI
  - `12px` softer cards
  - `16px` large cards / panels
  - `20px` emphasized rounded surfaces
  - `9999px` pills / full rounded shapes

### Rhythm rule

- Keep spacing and border radius visually consistent across blocks.
- Do not mix too many radius sizes in one screen.
- If the page is clean and institutional, stay tighter and more restrained.
- If the page is softer or more consumer-facing, increase radius gradually but keep the scale consistent.

## Default Output Style

Always present the result in this order unless the user asks otherwise:

1. `Boxed ASCII block layout` first
2. `Flow summary` second if useful
3. `Figma Make prompt` third if requested or clearly helpful
4. Markdown documentation only after the user approves

The default visual format is:

```text
┌─────────────────────────────────────────────────────────────┐
│  BLOCK X: NAME                                             │
│  ────────────────────────────────────────────────────────── │
│  GOAL                                                      │
│  ...                                                       │
│                                                            │
│  WHAT GOES HERE                                            │
│  ...                                                       │
│                                                            │
│  RECOMMENDED TEXT                                          │
│  ...                                                       │
│                                                            │
│  ACTION                                                    │
│  [KEEP] ... [MOVE] ... [ADD] ...                           │
└─────────────────────────────────────────────────────────────┘
```

When the user wants a Figma Make prompt or low-fidelity visual direction, apply these defaults:

- `WCAG Compliance`: use stronger contrast for labels, captions, and metadata so content meets or exceeds AA readability on white and light-gray surfaces.
- `Structural Visibility`: darken divider lines, borders, and arrow connectors enough that hierarchy and flow remain clearly visible in stakeholder presentations.
- Prefer dark grays over faint grays for structural text and separators.
- Avoid ultra-light dividers that disappear when screens are projected or shared.

## Core Workflow

### 1. Identify the page job

Figure out what the page needs to do first:

- explain the brand
- route audiences
- tell a story
- drive conversion
- provide utility
- build trust
- educate
- combine several of the above

For mobile, also identify:

- the screen's primary job
- whether the user is in a tab flow, onboarding flow, or task flow
- which actions need to be visible above the fold
- whether the screen is informational, transactional, or navigational

If the page has too many jobs, organize them into a clear top-to-bottom flow.

### 2. Define the flow before the blocks

State the page flow in plain language first.

Example:

```text
1. Hero
2. Audience routing
3. Product chapters
4. Proof
5. Education
6. Utilities
7. CTA
```

Mobile example:

```text
1. Header / context
2. Primary action
3. Key modules
4. Secondary actions
5. Navigation
```

Make the flow easy for stakeholders to discuss.

### 3. Turn the flow into boxed blocks

For each block, include:

- block name
- goal
- what content belongs there
- recommended text if the user wants content direction
- explicit labels like `KEEP`, `MOVE`, `ADD`, or `REMOVE` when restructuring an existing page

When the user already has content, also decide:

- which content deserves the largest box
- which sections need only a headline and one supporting line
- which blocks need a CTA placeholder
- which blocks need an image, illustration, or media placeholder
- which sections should stay quiet and utility-focused

For website layout work with existing content:

- do not just draw equal boxes for every section
- use layout weight to show importance
- use a small amount of content inside the box to explain its job
- keep the representation light enough that stakeholders focus on layout, not wordsmithing

For mobile screens, blocks may also represent:

- app bar
- KPI cards
- quick actions
- lists
- bottom sheets
- tab bars
- bottom navigation
- sticky CTAs

### 4. Keep fidelity intentionally low

Prioritize:

- clarity
- hierarchy
- sequence
- page logic
- stakeholder readability

Avoid:

- polished UI details
- color-heavy design direction unless requested
- high-fidelity component detail
- excessive copy length
- random spacing values that break rhythm
- inconsistent corner treatments across blocks

### 5. Offer Figma Make translation

When helpful, provide a Figma Make prompt that asks for:

- low-fidelity structure
- grayscale or black-and-white wireframe look
- stacked homepage or page blocks
- stakeholder-review readability
- block titles, purpose, and key content
- WCAG-friendly contrast for labels and metadata
- darker dividers, borders, and connectors for presentation visibility
- spacing that follows a clear 4px / 8px rhythm
- consistent border-radius choices across cards and panels

## Page Design Rules

- Start with the page's first job, not with random sections.
- Avoid turning every internal page or content family into a homepage block.
- Group related content into fewer, clearer chapters where possible.
- Separate `audience-based routing` from `need-based discovery` if both are necessary.
- Use proof early when trust matters.
- Use utilities later unless the page is primarily a service hub.
- If the user is restructuring an existing page, preserve important content but improve sequencing.
- Keep spacing consistent enough that the layout feels rhythmic rather than improvised.
- Use a restrained corner-radius system that supports the page tone.

## Suggested Block Types

Use only the block types that fit the page:

- Hero / opening promise
- Audience gateway
- Corporate proof / metrics
- Product chapters
- Need-state pathways
- Trust / security / reassurance
- Ways to use / channels
- Education / insights
- Utility / self-service
- Current promos / campaigns
- Group / ecosystem depth
- Pre-footer CTA
- Footer

Use only the block types that fit the mobile screen:

- App header / top bar
- Greeting / context
- KPI / status cards
- Quick actions
- Feature modules
- Feed / activity list
- Progress or onboarding steps
- Bottom navigation
- Utility / support actions
- Sticky CTA

## Figma Make Prompt Pattern

When generating a Figma Make prompt, ask for:

- low-fidelity page architecture
- clear stacked blocks
- grayscale or wireframe style
- minimal decoration
- strategic review readability
- section labels and short descriptions
- accessible contrast for labels, captions, and metadata
- dark enough borders, dividers, and connectors to keep hierarchy visible
- layout spacing aligned to a visible 8px rhythm with 4px sub-steps where needed
- card and container corner radii chosen from a small, consistent scale

Do not ask Figma Make for a polished final design unless the user explicitly wants that.

## Trigger Phrases

- "give me a block layout"
- "show me the page structure"
- "create a low fidelity homepage"
- "make this into a wireframe structure"
- "give me a boxed ascii layout"
- "turn this into a figma make prompt"
- "show what the page will look like"
- "organize this homepage"
- "create a stakeholder page blueprint"
- "show me the mobile app structure"
- "create a mobile screen blueprint"
- "give me a low fidelity app layout"
- "make this mobile flow into boxed ascii"

## Output Reminder

Default to:

- result first
- boxed ASCII format
- concise, structured, easy to review

Only convert to `.md` after the user is happy with the structure.
