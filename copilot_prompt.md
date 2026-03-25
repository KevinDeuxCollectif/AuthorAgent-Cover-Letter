# Copilot Prompt — Build the Cover Letter Agent GitHub Pages Site

Use this prompt in GitHub Copilot to generate the site. Paste the site_content.md file as context alongside this prompt.

---

## PROMPT

Build a single-page GitHub Pages site from the content in site_content.md. The site should be a clean, modern landing page that explains what the Cover Letter Agent is, how to set it up, and links to the agent instructions file.

### Technical requirements:
- Single index.html file (no build tools, no frameworks, no dependencies)
- Vanilla HTML + CSS + minimal JS (for smooth scroll and copy-to-clipboard)
- Hosted as GitHub Pages from the repo root
- Fully responsive (mobile, tablet, desktop)
- Fast loading — no external fonts, no images, no CDNs except optionally one icon set

### Design direction:
- Clean, editorial aesthetic. Not SaaS-startup. Not generic AI-tool.
- Light background (#f8f8f6 or similar warm off-white)
- Dark text (#1a1a1a) with muted secondary text (#555, #888)
- Cards with white backgrounds, subtle borders (#e0ddd6), rounded corners (10px)
- System font stack: -apple-system, BlinkMacSystemFont, 'Segoe UI', sans-serif
- Max-width content area (720px for text, 960px for wider sections)
- Generous whitespace between sections
- No hero images or illustrations — let the typography and structure do the work

### Page structure (map to site_content.md sections):

1. **Hero** — Title, tagline, one-sentence description, CTA button that scrolls to setup
2. **What It Does** — Three cards side by side (Score / Build / Score+Rebuild), each with icon, title, and 2-3 sentence description
3. **How It Works** — Four numbered steps with clear visual hierarchy. Step 3 includes a "Copy Instructions" button that copies the contents of agent_instructions.md to clipboard. Display a prominent link to the raw file as a fallback.
4. **What You Need Ready** — Simple three-column layout showing what to prepare for each mode
5. **The 10 Scoring Categories** — Vertical list of cards, each with category name, point value as a pill, and description paragraph
6. **Model Guide** — Table or card layout comparing Free/Pro Sonnet/Pro Opus/Max with expected scores, messages, and best-for guidance
7. **FAQ** — Accordion/collapsible sections
8. **About** — Brief paragraph on how it was built
9. **Footer** — Name, links, license

### Interactive elements:
- "Copy Instructions" button in the setup section — copies the full agent_instructions.md content to clipboard, shows "Copied!" confirmation
- Smooth scroll from hero CTA to setup section
- FAQ accordion (pure CSS or minimal JS)
- Sticky/fixed nav with section links (optional, only if it doesn't add complexity)

### The "Copy Instructions" button:
This is the most important interactive element. The agent_instructions.md file content should be embedded as a hidden element or JS string. When clicked, it copies the full text to the user's clipboard. Show a tooltip or text change confirming "Copied!" The button should be visually prominent — same styling as the hero CTA.

### Files to generate:
- index.html (the full site, self-contained)
- agent_instructions.md (the agent instructions file, linked for download and embedded for copy)
- README.md (brief repo readme pointing to the live site)
- LICENSE (MIT)

### Tone of the copy:
Direct, clear, no jargon. Written for someone who has never used Claude, has never created a Project, and is not technical. Every instruction should be concrete: "click this," "paste here," "type this." No assumptions about prior knowledge.
