# Product Marketing Context

**Document version:** v2
**Last updated:** 2026-09-09

## Product Overview
**One-liner:** An AI decision maker for iPhone and iPad that turns a hard, multi-factor choice into a clear ranked result in about ten minutes.
**What it does:** You add your options and the criteria that matter, weigh the criteria with quick pairwise comparisons (AHP), and score each option 1–5. Decisio computes a weighted ranking with a consistency check, and (Pro) an AI "Devil's Advocate" argues against your top pick — surfacing risks, blind spots, and hidden costs specific to your decision — plus an AI executive summary. It logs how the decision turned out and tracks a calibration score over time.
**Product category:** Decision-making / decision-support app. People search for "decision making app", "decision matrix app", "weighted pros and cons app", "how to choose between X and Y".
**Product type:** Consumer iOS app. iPhone + iPad, **iOS 17+**. On-device AI requires iOS 26+ (Apple Intelligence).
**Business model:** Free = 3 complete decisions, no account. Pro = $2.99/mo or $19.99/year (~44% off annual), **7-day free trial on the annual plan only**. Pro unlocks unlimited decisions, unlimited AI analysis, Devil's Advocate, AI executive summary, PDF/CSV (Excel) export, calibration tracking, Decision Playbook, priority support.

**AI is bring-your-own or on-device — not bundled.** Three modes (default "Smart/auto"): on-device via Apple Intelligence (iOS 26+, no key, fully private), or Cloud via the user's **own OpenAI API key** (gpt-4o-mini), or disabled. The core AHP method works with AI off. This is a real onboarding friction *and* a privacy selling point — see Objections.

## Target Audience
**Target companies:** N/A — B2C. Individuals making a specific high-stakes decision.
**Decision-makers:** The person facing the choice. Skews analytical / "overthinker" — people who already try to be rigorous (make lists, open a spreadsheet) and want something better than that.
**Primary use case:** A high-stakes decision with several real options and several competing factors, a deadline, and incomplete information — where a gut call feels risky and a pros/cons list isn't enough.
**Jobs to be done:**
- "Help me make this specific hard choice with enough confidence to stop second-guessing it."
- "Give me a rationale I can defend — to a partner, a boss, or myself in six months."
- "Challenge my gut pick before I commit to it."
**Use cases:**
- Which job offer to take (current paid-traffic focus)
- Where to live / which city to relocate to
- Big purchase: car, house, which apartment
- Hiring: which candidate
- Vendor / tool / contractor selection
- Any "Option A vs Option B vs stay put" fork

**⚠️ Positioning tension to resolve (central go-to-market decision).** The app *as built* leans **executive / business decision tool**: 9 of the 10 built-in templates are corporate (strategic planning, vendor selection, M&A, budget allocation, product decisions, business expansion, hiring, technology) — only "career" is personal. The AI rationale prompt literally says *"You are an executive decision advisor… focus on business impact, risk mitigation, and strategic alignment."* Onboarding, by contrast, is generic-personal ("stop overthinking"), and the paid niche test + much of the site target a **personal life decision** (job offer). Pick a lane per surface: the personal angle is the better paid-acquisition wedge (higher intent, less competition, an individual with a credit card), so the landing + ad + the job-offer flow should be unambiguously personal; the B2B breadth can stay as depth/SEO. Don't let the store listing and first-run read "corporate strategy tool" if the ads promise "which job do I take."

## Personas
N/A — single-stakeholder B2C purchase.

## Problems & Pain Points
**Core problem:** High-stakes decisions get made on gut feel plus one salient number (salary, price) plus a messy pros/cons list. The result is rumination before the decision and regret after it, because the factors that actually drive the outcome (manager quality, growth, hidden costs) got under-weighted against whatever was easy to compare.
**Why alternatives fall short:**
- Pros/cons lists: no weighting — a trivial con sits visually equal to a decisive one.
- Spreadsheets / weighted matrix: tedious to build, you invent the weights by typing percentages, nobody keeps them consistent across decisions, and there's no one to challenge the result.
- Asking friends: they don't know your criteria and anchor on the same salient number you do.
- Other decision apps: do the matrix math but stop there — no pairwise weighting, no adversarial check, no outcome tracking.
**What it costs them:** Days or weeks of rumination; a worse choice locked in for years (a job, a home); the specific regret of "I knew that mattered and I still let the big number win."
**Emotional tension:** Fear of choosing wrong on something irreversible; decision fatigue; the nagging sense that the choice is being driven by one number instead of the whole picture.

## Competitive Landscape
**Direct:** ChoiceMap, Decision Matrix, Best Decision (iOS decision apps) — they compute a weighted matrix but have no pairwise weighting, no AI challenge to the result, and no outcome/calibration tracking. Comparison pages exist at /compare/.
**Secondary:** Excel / Google Sheets weighted-decision-matrix template — powerful but tedious, weights are guessed, not reused, and it never pushes back on your answer.
**Indirect:** Pros/cons list, gut call, coin flip, crowdsourcing to friends, or decision paralysis (deferring the choice).

## Differentiation
**Key differentiators:**
- **AHP pairwise comparison** — compare criteria two at a time ("is growth more important than comp, and by how much?"), which produces more accurate weights than typing percentages, plus a consistency ratio that flags contradictory judgments.
- **Devil's Advocate AI** (Pro) — "a sharp, incisive decision analyst" that argues against your top-ranked option using *your own* criteria and scores: 3–4 specific risks, blind spots, hidden costs, and what the runner-up might do better.
- **On-device AI option** — Apple Intelligence mode means the AI features can run with zero data leaving the phone (iOS 26+).
- **Outcome tracking + calibration score** — logs how decisions turned out so your judgment improves over time; Decision Playbook stores reusable structures.
- **Built-in decision-science library** — the app ships a catalog of named methods and cognitive-bias explainers (anchoring, confirmation bias, sunk cost, recency, pre-mortem, regret minimization, opportunity cost, second-order effects, sensitivity analysis…). Reinforces "decision science, not vibes."
- **Method pedigree** — built on the Analytic Hierarchy Process; used in NASA, Boeing, and World Bank procurement; 100,000+ peer-reviewed papers since 1980.
**How we do it differently:** A structured method (not a blank grid) on your phone in ~10 minutes, with an AI that both helps build the model and attacks the conclusion.
**Why that's better:** Better weights → the decisive factors actually drive the ranking. The adversarial check → fewer regretted picks. Outcome tracking → the tool compounds in value.
**Why customers choose us:** They want rigor without building a spreadsheet, and they want something to pressure-test the answer, not just compute it.

## Objections
| Objection | Response |
|-----------|----------|
| "Isn't this just a pros/cons list?" | A pros/cons list has no weighting — a minor con looks as big as a decisive one. Decisio weighs the criteria against each other first, so the ranking reflects what actually matters to you. |
| "$20/year for something I'll use a few times a year?" | The decisions it's for — a job, a house — are the ones you live with for years. It's free for your first 3; you only pay if it's earning its keep. |
| "Do I have to bring my own AI key?" | The core method (weighting, ranking, consistency check) needs no AI. For AI help, on newer iPhones it runs on-device for free; otherwise you paste your own OpenAI key. Nothing is billed through us for AI. *(Friction: consider a bundled/managed AI tier later so this isn't a setup step.)* |
| "Will the math actually be trustworthy?" | It's the Analytic Hierarchy Process — the same method used in NASA and World Bank procurement — and it flags when your comparisons are internally inconsistent. The Devil's Advocate then argues against the result so you're not trusting it blindly. |
| "I can do this in a spreadsheet." | You can — then you maintain the spreadsheet, invent the weights, and have nothing challenge the answer. This is 10 minutes, guided, on your phone, with an adversarial check. |

**Anti-persona:** Someone who wants the app to *make* the decision for them; people optimizing low-stakes daily choices (what to eat, what to watch); anyone unwilling to spend ten minutes structuring the problem.

## Switching Dynamics
**Push:** Analysis paralysis on a live decision; regret from a past gut call driven by one number; spreadsheet fatigue.
**Pull:** A real method, on the phone, in ~10 minutes; an AI that both helps build the model and attacks the conclusion.
**Habit:** "I'll just think about it more" / reopening the same pros/cons note.
**Anxiety:** "Will this feel like homework?" "Will it take too long?" "Another subscription." "Do I need to set up an API key?" "What if the result contradicts my gut — do I trust it?"

## Customer Language
**How customers describe the problem:**
- ⚠️ *Need verbatim quotes — App Store reviews (0 so far), support emails, Reddit/Blind threads on "how to choose between job offers". This is the biggest gap in this doc.*
**How customers describe us:**
- ⚠️ *Need verbatim — no reviews yet.*
**Our own in-app voice (verbatim, for consistency — reuse this language on the site/ads):**
- "Stop guessing. Make confident decisions."
- "Tired of endless thinking and second-guessing?"
- "Turn complex choices into clear, data-driven decisions in minutes — not weeks. See exactly why one option wins."
- "What used to take days of endless thinking, you'll complete in 10 minutes."
- "Structured process eliminates analysis paralysis."
- "Stop relying on gut feeling alone."
- Devil's Advocate: "Expand to see the AI challenge your top choice." / "Analyzing blind spots…" / "Challenging: [your pick]"
- Paywall: "Decisio Pro — Unlock your full potential." / "Try Free — Then $19.99/yr."
**Words to use:** decide, ranked result, criteria, weigh, trade-offs, pairwise, pressure-test, gut check, blind spots, confidence, consistency check, "in about ten minutes", structured, "see exactly why one option wins", honest.
**Words to avoid:** "algorithm" (opaque), "optimize your life", generic AI-hype framing, "productivity", "life hack". Site/app voice is deliberately anti-hype — keep it. Also avoid over-corporate framing ("strategic alignment", "stakeholders", "executive") on personal-decision surfaces.
**Glossary:**
| Term | Meaning |
|------|---------|
| AHP | Analytic Hierarchy Process — pairwise-comparison weighting method, the app's engine |
| Pairwise comparison | Judging two criteria (or options) against each other at a time instead of scoring all at once |
| Consistency ratio | AHP check that flags when your pairwise judgments contradict each other (>0.1 = review) |
| Devil's Advocate | Pro AI feature that argues against your top-ranked option |
| Executive summary | Pro AI feature — plain-language write-up of why the winner won |
| Calibration score | Running measure of how well your past decisions predicted their outcomes |
| Decision Playbook | Pro feature — saved, reusable decision structures |
| Smart / On-Device / Cloud mode | AI provider setting: auto, Apple Intelligence only, or user's OpenAI key only |

## Brand Voice
**Tone:** Calm, direct, quietly contrarian. Treats the reader as smart and busy.
**Style:** Plain sentences, concrete numbers, no exclamation marks, no hype. Willing to concede a point ("Honest comparisons — even when another app wins").
**Personality:** Rigorous, grounded, candid, unpretentious, reassuring.

## Proof Points
**Metrics:** ⚠️ No usage/retention metrics worth citing publicly yet. Near-zero paid acquisition to date.
**Product claims already made in-app (keep consistent):** "~10 minutes per decision", "Save 3+ hours", "days of thinking → 10 minutes".
**Customers:** None nameable (B2C, early).
**Testimonials:** ⚠️ None — 0 App Store ratings. Do not fabricate. Path to first proof = in-app ratings prompt after a completed + rated decision (see iOS TODOs).
**Value themes:**
| Theme | Proof |
|-------|-------|
| The method is credible, not invented | AHP; NASA / Boeing / World Bank procurement; 100k+ peer-reviewed papers since 1980; in-app decision-science library |
| Fast, not homework | "A clear ranked result in about ten minutes"; 3 guided steps |
| It challenges you, not just computes | Devil's Advocate argues against your own top pick |
| Private if you want it | On-device Apple Intelligence mode — no data leaves the phone |
| Honest | Public comparison pages that concede where a competitor wins |

## Goals
**Business goal:** Grow Pro subscription revenue; keep the app in a state where it could be sold later.
**Conversion action:** Web → App Store download (tracked `app_store_click` / `app_store_clicked`) → in-app 7-day Pro trial start (`subscription_started`, `paywall_purchase_success`) → paid conversion.
**Current metrics:** Very low baseline traffic, near-zero paid acquisition. First paid test: $50 Google Ads, exact-match "job offer" keywords, landing on /decide/job-offer; decision threshold in the growth context.

## Changelog
*Newest first. One line per revision: what changed and why.*
- v2 (2026-09-09) — Rewrote against the actual iOS source (decision-ios repo). Corrected: iOS 17+ / on-device needs iOS 26+; **AI is BYO-OpenAI-key or on-device Apple Intelligence, not bundled** (new objection + anxiety). Added: verbatim in-app copy, on-device-privacy differentiator, in-app decision-science library, real Devil's Advocate framing. Flagged the **B2B-executive vs personal-life positioning tension** (9/10 built-in templates + the AI rationale prompt are corporate; ads/landing are personal) as the central GTM decision.
- v1 (2026-09-09) — Initial context, auto-drafted from the website repo + session positioning.
