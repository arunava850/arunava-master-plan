# LinkedIn posts

## Status key
- `[ ]` Not written yet
- `[draft]` Written, needs review
- `[ready]` Ready to publish
- `[published]` Live — add date
- `[pending approval]` Waiting on intro post publication before scheduling

---

## Post 0 — Pinned intro post
**Status:** `[ready]` — APPROVED April 22, 2026
**Type:** Pinned profile post
**Publish:** As soon as you approve (publish + pin immediately)

I've been building for months and telling nobody.

A comment system for online art courses. UI screens from Figma using Cursor. Cricket analytics dashboards. Small tools, real problems, shipped quietly.

Why? Because I wasn't sure if any of it was worth sharing.

But here's what I learned: the best way to learn is to build in public. Not for clout. Not for the algorithm. Just because it forces you to be honest about what works and what doesn't.

So I'm changing that.

Starting now, I'm documenting what I build — the wins, the failures, the honest decisions. No filters. No "perfect" projects. Just real work.

Why should you care?

→ If you're building AI tools, you'll see how I'm using Cursor and Claude to ship faster
→ If you love cricket, you'll see data insights nobody's talking about
→ If you're an artist or creator, you'll see how I'm thinking about platforms that help artists make money

20 years of enterprise systems taught me one thing: the real value is in the *building*, not the resume.

Let's build together.

What are you working on right now?

#Building #AI #Cricket #ShippingCode

---

## Post 1 — Comment System for Courses (The Build)
**Status:** `[draft]` — Ready to expand
**Type:** Build post
**Publish:** Within 2 weeks of intro post (likely end of April)
**Hook:** "I built a custom comment system for online courses — and it's way simpler than you'd think"

---

**Framework:**

I just finished building a comment system for Debasree's online art courses. It's live, it's working, and it taught me something important about constraints.

**The problem:**
Standard course platforms (Teachery, Kajabi) don't let you embed discussions at the module level. Students can't ask questions about *this specific lesson*, only about the course overall. For art courses where each module is a different technique, that's broken.

**What I built:**
A lightweight comment widget that:
- Sits below each course module
- Stores comments in a simple database
- Notifies Debasree when a student asks a question
- Lets her reply directly in the module thread

Nothing fancy. No ML. No real-time sync. Just comments that work.

**What surprised me:**
I kept trying to overthink it. Custom databases, authentication libraries, all these abstraction layers. But then I realized: I'm using Claude for the heavy lifting. The comment system itself could be dead simple. Let the AI handle the complexity, keep the core tool minimal.

**Why it matters:**
This is the pattern I'm seeing everywhere now — the modern stack is: simple foundation + AI where it counts + students stay focused.

**What's next:**
Sending this to two other course creators Debasree knows. Hoping one turns into a second reference site for the Dear Art service.

#BuildingInPublic #AITools #OnlineCourses

---

## Post 2 — Comment System for Courses (The Learning)
**Status:** `[draft]` — Ready to expand
**Type:** Learning post / deep dive
**Publish:** Following week (within 10 days of Post 1)
**Hook:** "Building a course comment system taught me why constraints are the best design tool"

---

**Framework:**

Most of the work building the comment system wasn't the coding. It was saying no.

No real-time notifications (polling is fine). No user mentions. No nested replies (flat threads work). No markdown (students won't use it). No emoji reactions. No moderation AI (Debasree reviews everything).

Each constraint I added made the system *better*, not worse. Fewer features = faster to build = easier to debug = students understand it immediately.

This is the opposite of how I used to build in the enterprise world. More features = more value. More sophistication = more worth.

But with AI tools changing the game, I'm learning the formula flips:

**Constraint → Clarity → Simplicity → Speed → Audience clarity**

When the foundation is dead simple, you can add complexity where it actually matters. Not in the comment system itself. In what Claude does with those comments.

Next build: using those same comments as training data for a course Q&A bot. The comment system doesn't need to be smart. It just needs to feed data to something that is.

#BuildingInPublic #SystemsThinking #ProductDevelopment

---

## Post 3 — Figma to Code with Cursor (The Workflow)
**Status:** `[draft]` — Ready to expand
**Type:** Build post — process focused
**Publish:** 1-2 weeks after Post 2
**Hook:** "I just converted Figma designs to production HTML/CSS in 90 minutes. Here's how."

---

**Framework:**

One of the common gripes from designers I work with: "I design in Figma, engineer builds in React, and the hand-off is messy."

I just tested a workflow that cuts that problem in half.

**The process:**
1. Designer exports Figma components as SVG or high-res PNG
2. I screenshot the design in Figma (whole page view)
3. Paste screenshot into Claude context
4. Use Cursor to have Claude write the HTML/CSS to match it
5. Claude generates component-based code ready for integration

**Time:** 90 minutes for a 5-section landing page

**What worked:**
Cursor's multi-file editing. I had Claude write the base HTML, refine the CSS, extract reusable components, and add interactivity — all in one workflow. Zero browser tab switching.

**What didn't:**
Shadows and gradients. Claude guesses well but doesn't match Figma's exact values. Still had to tweak those manually.

**The insight:**
This isn't replacing designers. It's replacing the "exported component library that nobody uses" part. Designers stay in Figma. I stay in code. Figma → screenshot → Claude → code works.

We're using this at Ainsemble now for rapid UI prototyping. One designer, one engineer, 90 minutes = working prototype.

#BuildingInPublic #DesignSystems #CursorAI

---

## Post 4 — Figma to Code with Cursor (The Deep Dive)
**Status:** `[draft]` — Ready to expand  
**Type:** Learning post / system design
**Publish:** 1 week after Post 3
**Hook:** "Why Figma → screenshot → Claude → code is replacing design-to-dev handoffs"

---

**Framework:**

The old design-to-dev workflow assumed a translation problem: designer makes beautiful mockup, engineer builds it, there's always a gap.

But that assumes the engineer is the bottleneck. What if the real bottleneck is the *communication*?

**The old way:**
Designer → Figma file → export components → engineer reads spec → engineer builds → three rounds of fixes

**The new way:**
Designer → Figma mockup → screenshot + one question → Claude → code → one tweak → done

The key change: Visual + context beats written specification every single time.

Claude (and now Cursor) can look at a screenshot and write code that matches it with ~90% accuracy. The 10% (shadows, exact spacing) takes 10 minutes to fix manually. Faster than going back to the designer, asking questions, waiting for clarification.

**Why this works:**
Visual input bypasses the language problem. Claude doesn't need to read "button should have 16px padding with a subtle shadow" — it can see the button and infer most of it.

**Where it breaks:**
- Interactions Claude can't see in a static image (hover states, animations)
- Exact color values (Claude guesses, but screenshots compress color)
- Responsive behavior (screenshot is one breakpoint)

For the last part, that's where the engineer's judgment still matters. Claude gets you 80% there on responsive logic, you tune the last 20%.

**The meta take:**
This is what's shifting across all workflows right now. Not "AI replaces engineers." It's "AI handles the parts that required manual translation, engineers focus on the 10% that needs judgment."

Designers can ship faster. Engineers focus on harder problems. Both win.

#BuildingInPublic #DesignSystems #AIProductivity #FrontendDevelopment

---

## Weekly rhythm

| Day | Post type |
|---|---|
| Monday | Build post — something shipped |
| Wednesday | Learning post — something figured out |
| Friday | Cricket analytics update |

---

## Post schedule — Next 3 weeks

**Week 1 (Post intro):**
- Mon: Post 1 — Comment system build
- Wed: Post 2 — Comment system learning
- Fri: Cricket update (from Q8 answer — depends on Day 1 build)

**Week 2:**
- Mon: Post 3 — Figma to code workflow
- Wed: Post 4 — Figma to code deep dive
- Fri: Cricket update

**Week 3+:**
- Establish rhythm based on Day 1 launch and build momentum
