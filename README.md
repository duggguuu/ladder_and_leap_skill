# Ladder & Leap

**An end-to-end brand strategy and copywriting skill for brand managers, built for [Claude Code](https://claude.com/claude-code) and Claude.ai.**

Positioning theory and Madison Avenue-grade craft, packaged as a working system — not a thin AI wrapper around "write me some marketing copy."

## Why this exists

Most AI marketing prompts default to generic startup-blog voice: safe, adjective-heavy, indistinguishable from every other brand's output. This skill exists because real brand work isn't generic — it's built on decades of hard-earned strategic theory and craft discipline that most AI tooling simply ignores. **Ladder & Leap** packages that discipline into something you can actually run a real brand task through: position a product against a real competitive ladder, brief creative work tightly enough that it doesn't come back wrong, write headlines using named techniques from the people who actually invented modern advertising, and audit a campaign before it ships instead of after it flops.

It was built by Yash Gohel, a Brand Manager at Zydus Wellness (TatvaCare / GoodFlip) with roughly six years across healthtech, fintech, and DTC marketing — as the tool he actually wanted to use on the job, then shared publicly because it turned out to be useful beyond one team.

**Ladder**, because positioning means knowing exactly which rung of the category ladder you're claiming, and having the discipline not to fight for one you can't hold. **Leap**, because a correct strategy isn't the same thing as work anyone remembers — somewhere between the brief and the finished ad, someone has to make the creative leap.

## What it does

- **Positions a brand or product** using a category-ladder framework, leader/follower strategy, and a one-line positioning-statement generator.
- **Defines a brand voice system** with a tone-of-voice matrix and a "say it, don't describe it" method instead of another adjective-only style guide.
- **Tightens creative briefs** with a one-page template and a five-question tightness test that catches feature lists and mission statements disguised as strategy.
- **Develops and reviews creative work** using a Hegarty-inspired framework for briefing fearlessly and running reviews that don't sand strong ideas down to safe.
- **Writes and diagnoses headlines and campaign copy** using twelve named, real, historically documented techniques from legendary copywriters — David Abbott, Dave Trott, Neil French, Dan Wieden, Ed McCabe, and more.
- **Audits offers and campaigns** before launch (or diagnoses them after) with an original Five Fit Checks scoring framework, plus a post-mortem template.
- **Structures go-to-market plans** — messaging hierarchy, launch phasing, and a channel-mix logic tied back to your actual ladder position.
- **Ships a ready-to-paste prompt library** so you can skip the reading and get straight to work.

## Structure

```
ladder-and-leap/
├── SKILL.md                              # Entry point: overview, routing table, operating principles
├── README.md                             # You are here
└── reference/
    ├── 01-positioning.md                 # Category ladders, leader/follower strategy, positioning worksheet
    ├── 02-brand-voice-system.md          # Voice matrix, content cadence system, consistency audit
    ├── 03-creative-brief.md              # One-page brief template + tightness test
    ├── 04-creative-development.md        # Briefing fearlessly, running reviews, the creative review filter
    ├── 05-copywriting-canon.md           # 12 named techniques from real, documented campaigns
    ├── 06-offer-and-campaign-audit.md    # The Five Fit Checks + post-mortem template
    ├── 07-go-to-market.md                # Messaging hierarchy, launch phasing, GTM one-pager
    └── 08-prompt-library.md              # Ready-to-paste prompts for every stage above
```

Each reference file works standalone — you don't need to read the whole skill to use one piece of it. `SKILL.md` is the router: it stays short and tells Claude (or you) which file to pull for a given task, in the spirit of progressive disclosure.

## Installation

### Option 1 — Claude Code (recommended)

Clone straight into a skills directory. Project-level makes it available only inside that project; user-level makes it available in every Claude Code project you open.

```bash
# project-level (this project only)
git clone https://github.com/YOUR-USERNAME/ladder-and-leap.git .claude/skills/ladder-and-leap

# user-level (every project)
git clone https://github.com/YOUR-USERNAME/ladder-and-leap.git ~/.claude/skills/ladder-and-leap
```

No build step, no config. Start (or restart) Claude Code and the skill is live — Claude reads `SKILL.md` automatically once it's in a skills directory.

### Option 2 — Claude.ai (Projects)

1. Download this repo (Code → Download ZIP, or `git clone` it) and unzip it.
2. Open a Claude.ai **Project** → **Project knowledge** → **Add files**.
3. Upload the whole folder — or, at minimum, `SKILL.md` plus whichever `reference/*.md` file your task needs.
4. Prompt normally in that project; Claude will use the uploaded files as context.

### Option 3 — No install, just paste

Don't want to set anything up? Open `reference/08-prompt-library.md` in this repo, copy the block for the stage you're on, fill in the brackets, and paste it into any Claude conversation.

## How to use it

Once it's installed, just describe what you're doing in plain language — you don't need to name a file or a framework:

- "Help me position this product against [competitor]"
- "Review this creative brief before I send it to the agency"
- "Give me ten headline directions for [product]"
- "Audit this campaign before we launch it"
- "Build a tone-of-voice guide for [brand]"
- "Plan the go-to-market for this launch"

Claude reads `SKILL.md` first — the router — and pulls only the specific reference file your task needs, rather than dumping the whole skill on you at once. If you're not sure where to start, say so; the same routing table Claude uses is right here:

| You're trying to... | Go to |
|---|---|
| Figure out where your brand/product stands, or should stand, in the customer's mind | `reference/01-positioning.md` |
| Define or tighten how your brand sounds, in every piece of copy, everywhere | `reference/02-brand-voice-system.md` |
| Turn a strategy into a brief a creative team (or Claude) can actually work from | `reference/03-creative-brief.md` |
| Review, unblock, or push back on creative work without killing it | `reference/04-creative-development.md` |
| Write or diagnose headlines, campaign lines, or long-form copy | `reference/05-copywriting-canon.md` |
| Stress-test an offer or a finished campaign before it goes live, or diagnose why one underperformed | `reference/06-offer-and-campaign-audit.md` |
| Plan a launch — messaging hierarchy, phasing, channel mix | `reference/07-go-to-market.md` |
| Skip the reading and just get straight to work with a ready-made prompt | `reference/08-prompt-library.md` |

Each reference file works standalone, so this isn't all-or-nothing — pulling just `05-copywriting-canon.md` for a headline session is a completely normal way to use this.

## Credit and inspiration

This skill draws on real, published frameworks and real, documented advertising history, rewritten in its own words — it does not reproduce any source text verbatim.

- Positioning frameworks are inspired by **Al Ries and Jack Trout, *Positioning: The Battle for Your Mind*** (McGraw-Hill).
- The creative-development framework is inspired by **John Hegarty, *Hegarty on Creativity: There Are No Rules*** (Thames & Hudson).
- The copywriting canon draws on the craft and real career histories of legendary copywriters whose work is collected in **D&AD and TASCHEN's *The Copy Book*** — among them David Abbott, Dave Trott, Neil French, Dan Wieden, Ed McCabe, Bob Levenson, Indra Sinha, John Bevins, Steve Hayden, Janet Kestin, Jeremy Sinclair, Sean Doyle, Tim Delaney, Mike Lescarbeau, Dan Germain, and Nick Asbury.

Read the originals — this skill is a companion and a working toolkit, not a substitute for any of them.

## License

MIT. Use it, fork it, adapt it for your own brand or agency. See `LICENSE`.
