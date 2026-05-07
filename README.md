# SOW Reviewer for SMB Home Services Agencies

A reviewer for SOW and scope documents at solo-to-small digital agencies serving SMB home services clients. Run it in Claude Code, point it at a draft SOW, and get back a diagnostic review — flags, failure modes, and specific revision directions.

This folder is built for Claude Code, where the routing architecture loads files on demand based on the task. The methodology — each file does one job, the structure routes Claude's attention to what's relevant — works as designed in Claude Code. It can be adapted for claude.ai projects by adding all files to project knowledge, but the load/skip discipline is sharper in Claude Code.

## Who this is for

Solo-to-small agency owners (1–5 people) who write SOWs for SMB home services clients (roofing, HVAC, plumbing, lawn care, similar). The reviewer understands the operational realities of this audience — owner-operator dynamics, seasonality, lead-quality blame games, the relationship between handshake culture and contract language — and reviews accordingly.

If you run a different kind of agency or serve a different audience, the diagnostic frameworks will still apply, but the audience-specific commentary won't fit your context.

## Prerequisites

- [Claude Code](https://docs.claude.com/en/docs/claude-code) installed and working in your terminal.
- An Anthropic API key or Claude subscription that supports Claude Code.

If you've never used Claude Code, the setup takes about five minutes — see Anthropic's docs linked above.

## How to use it

1. **Clone or download this repo:**

   ```bash
   git clone [repo-url]
   cd sow-reviewer
   ```

2. **Open Claude Code in the folder:**

   ```bash
   claude
   ```

3. **Ask Claude to review your SOW.** Two ways to do this:

   - **Reference a file in the `drafts/` folder.** Save your draft SOW as a markdown or text file in `drafts/` (e.g., `drafts/my-client-sow.md`), then tell Claude: *"Review the SOW in drafts/my-client-sow.md"*
   - **Paste the SOW directly.** Tell Claude: *"Review this SOW:"* followed by the SOW text pasted into your message.

4. **Choose your output format.** Before producing the review, the reviewer will ask whether you want a quick terminal output or a written review file saved to `reviews/`. Pick whichever fits your workflow — terminal for fast feedback, written file when you want to keep or share the review.

5. **Push back where you have context the reviewer doesn't.** The reviewer will name the risks you're accepting and defer on the decision. It won't fold to social pressure, but it respects your business context when you provide it.

## Try it out immediately

Two sample SOWs are included in `drafts/` so you can test the reviewer before working with a real document:

- `drafts/sample-northstar-roofing-sow.md` — a web project SOW (website redesign for a roofing company)
- `drafts/sample-coastal-comfort-sow.md` — a hybrid SOW (website redesign + CRM setup + post-launch retainer for an HVAC company)

Open Claude Code in this folder and tell it: *"Review the SOW in drafts/sample-northstar-roofing-sow.md"* (or *"...in drafts/sample-coastal-comfort-sow.md"*). Replace or delete the samples whenever you're ready to use your own SOWs.

## What you get back

A structured diagnostic review, organized by severity:

- **Critical flags** — issues that will likely cause disputes, scope creep, or relationship damage if the SOW is sent as written
- **Significant gaps** — issues that should be fixed before sending but aren't yet causing harm
- **Minor refinements** — language tightening, formatting suggestions, optional improvements
- **Closing summary** — the single highest-priority fix to make before sending

Each flag names the clause, the failure mode it creates, and a specific revision direction. The reviewer is opinionated and direct — it won't soften flags to be polite, and it won't return "looks good" without explanation.

What it does *not* return: a polished rewrite of your SOW. The output is a diagnostic, not a redraft. You make the revisions yourself, with the reviewer's reasoning in front of you.

## What this doesn't do

- **Lead-generation retainers.** Ad campaign scoping has its own attribution traps that need a different specialist.
- **Data import and CRM cleanup.** Messy data engagements deserve their own scoping logic.
- **SEO scope language.** SEO deliverables fail in unique ways that need specialist treatment.
- **Implementation guidance.** This is a reviewer, not a builder.
- **Legal enforceability.** The reviewer covers operational craft (will this prevent disputes?), not legal validity (will this win in court?). For legal review, see a lawyer in your jurisdiction.

If your SOW falls into one of these categories, the reviewer will tell you and decline to proceed.

## How the folder works

The folder uses a layered structure so different parts of the reviewer apply to different parts of the SOW. Identity, response rules, and the two foundational reference files (deliverable-language-patterns, smb-home-services-context) inform every review. Trigger-based reference files (red-flag-catalog, pricing-and-ownership) come into play when the SOW contains language those files are built to catch.

You don't need to manage what's used when — Claude reads the folder structure and applies the relevant frameworks based on the SOW in front of it.

## Files

```
sow-reviewer/
├── CLAUDE.md                          ← entry point Claude reads first
├── README.md                          ← this file
├── identity.md                        ← who the reviewer is, what it covers, what it believes
├── rules.md                           ← how the reviewer responds and behaves
├── examples.md                        ← three worked example reviews showing the reviewer in action
├── reference/
│   ├── deliverable-language-patterns.md  ← the diagnostic frameworks (always loaded)
│   ├── smb-home-services-context.md      ← the audience-specific lens (always loaded)
│   ├── red-flag-catalog.md               ← scannable pattern library for fast pass
│   └── pricing-and-ownership.md          ← deep-dive on pricing models and account ownership
├── drafts/
│   ├── sample-northstar-roofing-sow.md   ← web project sample SOW
│   └── sample-coastal-comfort-sow.md     ← hybrid (web + CRM + retainer) sample SOW
└── reviews/
    └── (reviewer writes reviews here when you choose file output)
```

## Where to start

If you want to see what the reviewer does before using it, read [examples.md](./examples.md) — three worked reviews across web project, marketing ops, and maintenance retainer SOWs.

If you want to use the reviewer immediately, follow the steps in **How to use it** above. Try it on either sample SOW in `drafts/` first.

---

Built using folder-based specialist methodology — each file does one job, and the structure routes the reviewer's attention to what's relevant.
