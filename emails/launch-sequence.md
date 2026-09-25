# Jevline™ — 3-Email Launch Sequence

From: The Jevline Team <gentledesk632@agentmail.to>
Product: The Typed Decision Playbook™ — 8 PDFs, $19 founder
Voice: plain-spoken, engineering-credible, zero hype-words, one idea per paragraph.

---

## EMAIL 1 — TEASER (send 48h before launch)

**Subject:** the 0.9 in every Jev example is a lie

**Preview:** (it's a teaching number, not a measured one — here's what to do instead)

**Body:**

Hey — quick one.

If you've copy-pasted a Jev quick start in the last two weeks, you inherited this line:

```
const action = p >= 0.9 ? "route" : "review";
```

That `0.9` has been copied into a thousand codebases. Almost nobody has *measured* it.

It's a teaching number. It appears in the docs to illustrate a *shape* — "threshold, then branch" — not to recommend an operating point. Your traffic isn't the docs' traffic. Your error costs aren't theirs.

Here's the uncomfortable part: **a threshold you haven't plotted on your own labelled cases is a threshold you don't own.**

So when someone on the team asks "why 0.9?" — the honest answer is "because the README said so."

Thursday I'm sending you the fix: **The Typed Decision Playbook™** — an 8-part system for shipping Jev decisions you can actually defend.

One idea to take away today:

> Ask **facts**, not decisions.
> The model answers "was a refund requested?"
> *Your code* decides whether to grant it.

That one split removes most of the risk people are quietly shipping right now.

Talk Thursday.

— The Jevline Team

P.S. If you want the 30-minute version early, reply with the word **THRESHOLD** and I'll send the calibration one-pager before launch.

---

## EMAIL 2 — LAUNCH (send on launch day)

**Subject:** it's live: ship a verdict, not a vibe

**Preview:** The Typed Decision Playbook™ — 8 PDFs, $19 founder price

**Body:**

It's live.

**Jevline™ — The Typed Decision Playbook™**
→ 8 PDFs, $19 founder price (anchor $196)
→ https://jevline.vercel.app/

Here's the whole idea in four words:

> **ASK → SHAPE → CALIBRATE → GATE.**

**ASK** — one narrow, independent question. Never the mega-question that bundles five judgments and averages them into mush.

**SHAPE** — pick the answer your code can consume. Noul for gates. Choice for routers. Score for ranking. If you're parsing strings, you picked wrong.

**CALIBRATE** — freeze the decisions, sweep the threshold, plot false-auto-route against review load, then quote the *holdout* number you never tuned on.

**GATE** — ALLOW / REVIEW / REFUSE. Never a bare yes/no. When in doubt, do the reversible thing.

What's inside (all 8):

1. The Typed Decision Playbook — the core guide
2. The Question Shaper + Primitive Selector — Noul / Choice / Score done right
3. The Threshold Calibration Kit — sweep it, plot it, defend it
4. Abstention & Escalation Design — make "I don't know" useful
5. The Cascade & Cost Blueprint — when a bigger model actually pays
6. The Decision Ledger + Drift Watch — catch drift before your users do
7. The Failure-Mode Playbook — 7 ways it breaks + the exact fix
8. The 30-Day Rollout Playbook — one step → an owned decision layer

**The part that matters most:** the failure modes nobody tells you about.

Independent gate studies keep finding that the biggest source of *wrong decisions* isn't the model — it's the **action-mapping** code around it. The label was right and the action was wrong. Same for cascades that cost 47% more and fix nothing, because the uncertainty was missing information, not hard reasoning.

Jevline gives you a test for each one.

→ **Get The Typed Decision Playbook — $19** (60-day guarantee, keep it either way)
→ https://jevline.vercel.app/

Your LLM writes the words. A typed decision gives it a judgment you can test, price, and trust.

**Don't ship a vibe. Ship a verdict.**

— The Jevline Team

---

## EMAIL 3 — FOLLOW-UP (send 48h after launch)

**Subject:** "but my step is too simple for a whole system"

**Preview:** good — that's exactly where this pays fastest

**Body:**

The most common reply so far: *"My decision step is simple. Do I really need all this?"*

Yes — and faster than you'd think.

Simple steps are where this pays because the downside is invisible. You have a string match like:

```js
const urgent = ticket.body.includes("asap") || ticket.body.includes("urgent");
```

It works. Until it doesn't. Someone writes "no rush, whenever" and it flags urgent. Someone writes "I'm losing sales" and it misses entirely. You never see it, because there's no log and no number — just a vague sense your triage is a bit off.

Swap it for one Noul question:

```js
urgent: noul("Does the message explicitly mention losing money or a deadline?")
```

Now you have a **probability**. Now you can:
- **sweep a threshold** and know your error rate on real cases,
- **route the uncertain ones to review** instead of guessing,
- **log every decision** so you can prove it works next month.

That's a real decision layer for one afternoon's work. And it's exactly what deliverable 1 walks you through, start to finish.

**The launch price is $19 through this weekend** — after that it goes to the standard price.
→ https://jevline.vercel.app/

And the guarantee stands: 60 days, no questions, keep the PDFs either way. If the Failure-Mode Playbook doesn't save you one bad deploy, tell me and I'll refund you.

— The Jevline Team

P.S. The single highest-leverage page in the whole pack is the **cascade cost table** — it's the difference between "escalate to the big model" being nearly free (5% of traffic) and a 2.6× tax (40%). Worth the price on its own.
