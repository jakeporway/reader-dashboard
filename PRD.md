# the curator's Curation Lab — Product Requirements Document

## Vision
A personal curation dashboard that helps the curator discover, evaluate, and share inspiring content from across the internet. The goal is to cut through the noise and surface genuinely interesting, underreported stories at the intersection of creativity, innovation, human-centered design, art & science, behavioral economics, social impact, and what it means to be human today.

## The Human
**the curator** — Works in innovation, consulting, HCD, design, research, strategy, decision-making, and entrepreneurship. She's art-forward, socially conscious, and deeply curious. She wants to feel inspired and share that inspiration with friends and colleagues.

## The Problem
It's really hard to find valuable, interesting content online. There's too much noise, too many surfaces, and the truly fascinating stuff gets buried. the curator wants a curated feed of the good stuff — the things that make you stop and think, that connect unexpected dots, that inspire creativity and hope.

## The Solution
A two-part system:

### Part 1: JawnBot Daily Curation (AI-powered)
- **Daily Pull**: Each morning, JawnBot scans ~95 curated sources and surfaces ~20 links for the curator to review
- **For each link, JawnBot provides:**
  - A punchy, curiosity-driven headline (scannable, email-ready — not just the article title)
  - A 2-3 sentence description: what it is, why it's interesting, connections to broader themes
  - Topic category tags
  - Alignment score (1-5) based on the curator's interests
  - Paywall flag
- **Learning loop**: the curator rates content (🔥👍😐👎) and leaves comments. Over time, JawnBot refines its curation algorithm based on her feedback patterns — tone, depth, medium, topic gravity, novelty threshold.
- **Ongoing source discovery**: JawnBot proactively finds new sources based on what the curator gravitates toward.

### Part 2: The Dashboard (Web App)
A private, bookmarkable website with four views:

1. **📰 Daily Feed** — List view of each day's curated links with headlines, descriptions, topic tags, alignment scores. Rating buttons (🔥👍😐👎) and comment fields on every item.

2. **📌 Board View** — Pinterest-style visual grid layout for browsing. Good for getting a visual sense of the day's content.

3. **⭐ Favorites** — Filtered view of everything rated 🔥 or 👍. the curator's personal archive of the best stuff.

4. **✍️ Draft Builder** — Auto-compiles favorites into a copy-pasteable format for Substack/Instagram. the curator can review, edit, and publish.

**Additional features:**
- Topic filter chips for narrowing by category
- Export feedback as JSON (so JawnBot can analyze patterns)
- All feedback stored in browser localStorage (private, no backend needed)
- Clean, minimal design — feels calm, not overwhelming

## Content Categories (Source Database)
~95 sources organized into 12 categories:
- 🎨 Art, Design & Creative Practice
- 🔬 Art & Science Intersection
- 🧠 Behavioral Science, Psychology & Human Behavior
- 💡 Creativity, Innovation & Entrepreneurship
- 📊 Data Visualization & Visual Research
- 🔧 Design Methodology, HCD & Research
- 🌍 Social Impact, Systems Change & Civic Design
- 🔮 Systems Thinking, Futures & Strategy
- 🤔 Unusual Perspectives & Deep Thinking
- 📚 Technology with a Human Lens
- 🤪 Weird, Funny & Wonderful Internet
- 🎮 Interactive Experiences & Creative Projects

Full source list maintained in: `curator-newsletter-master-sources.md`

## the curator's Content Preferences (Evolving)
Based on initial feedback:
- LOVES: Creative process & methodology, art+science intersections, interactive/playable experiences, speculative design, systems thinking with soul, social impact through design
- Specifically excited by: Creative Applications Network (process/iteration focus), Emergence Magazine, Are.na, Dark Matter Labs, Civilla, Nicky Case
- NOT looking for: Heavy AI/ML art focus, mainstream tech news, anything supporting Trump/MAGA
- Wants VARIETY: innovation, consulting, HCD, design, research, strategy, entrepreneurship, behavioral economics — plus wildcards and surprises
- Values: diverse voices, global perspectives, things that go past the surface, hopeful and inspiring but not shallow

## Output Channels
the curator plans to share curated content via:
- **Substack** — Weekly newsletter with ~5-10 links, each with a short engaging blurb
- **Instagram** — Visual/bite-sized version (format TBD)

## Workflow
1. **Morning**: JawnBot posts daily pull (~20 links) to the dashboard
2. **Throughout the day**: the curator browses, rates, comments
3. **End of week**: the curator reviews favorites in Draft Builder, edits, publishes to Substack/Instagram
4. **Ongoing**: JawnBot learns from feedback, discovers new sources, refines curation

## Technical Architecture
- **Frontend**: Single-page HTML/CSS/JS app (no framework needed)
- **Data**: JSON file (`data.json`) updated daily by JawnBot
- **Storage**: localStorage for ratings/comments (client-side only)
- **Hosting**: GitHub Pages (jakeporway.github.io/reader-dashboard)
- **Updates**: JawnBot pushes new data.json daily via git

## Current Status
- ✅ Source database compiled (~95 sources across 12 categories)
- ✅ Dashboard v1 built (all 4 views working)
- ✅ First content pull complete (38 links from 14 sources)
- ✅ Deployed to GitHub repo
- 🔲 GitHub Pages needs to be enabled
- 🔲 the curator's first round of feedback (to calibrate curation)
- 🔲 Daily automated pull workflow
- 🔲 Substack/Instagram template design
- 🔲 Source feed integration (RSS/archive browsing)

## Future Ideas
- RSS feed aggregator built into the dashboard
- Visual article previews (thumbnail images)
- Search/filter across all past pulls
- "Surprise me" random discovery mode
- Collaboration features (if the curator wants to co-curate with others)
- Auto-draft Substack posts from favorites

---
*Built by JawnBot ⚡ for the curator, February 2026*
