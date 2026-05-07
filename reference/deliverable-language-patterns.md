# deliverable-language-patterns.md

Five tests the specialist runs against every SOW. Each one is structural — a real diagnostic, not a checklist of language to avoid. Pattern-matching shortcuts ("as needed," "ongoing optimization," "best practices") live in `red-flag-catalog.md`. This file holds the tests that work even when the SOW is using language no catalog has seen before.

---

## The quantity/cadence/acceptance test

Every deliverable line in an SOW must answer three questions. If it can't answer all three, it's not a deliverable — it's a deferred conflict.

**Quantity.** How many of this thing get produced? "12 ad variations." "4 blog posts." "1 design system." "Up to 3 integrations."

**Cadence.** How often, on what rhythm, by when? "Per month." "By week 4 of the engagement." "Within 5 business days of receiving final assets." "Twice during the build phase."

**Acceptance.** Acceptance has two parts, and both must be specified.

- **Functional acceptance** — what objectively makes this thing complete? "Form submits successfully across Chrome, Safari, Firefox on desktop and mobile." "Dashboard reflects accurate data from connected sources." "Integrations pass test events end-to-end." This is the technical bar.
- **Procedural acceptance** — how is completion confirmed between agency and client? "Client reviews and confirms in writing within 5 business days." "Demo walkthrough during weekly call." "Automated test results delivered with the build." This is the sign-off mechanism.

Both are required. A deliverable with procedural acceptance but no functional acceptance is still unbounded — "client confirms in writing" can mean anything if there's nothing concrete to confirm. A deliverable with functional acceptance but no procedural acceptance leaves the agency uncertain whether the client agrees the bar was met.

Any deliverable missing any of the three (quantity, cadence, or either side of acceptance) is a flag. The fix is naming the missing dimension explicitly, not hand-waving with "as needed" or "ongoing."

### The principle behind the test: bounded vs. unbounded

The dichotomy that matters isn't activity vs. artifact. It's bounded vs. unbounded.

A "monthly review call" is technically an activity, not an artifact — but it's a fine deliverable because it has edges. One call, monthly, defined participants, defined agenda. The activity has a quantity, a cadence, and acceptance criteria built in.

By contrast, "monthly check-ins as needed" is also activity-shaped, but it's unbounded. "As needed" defeats the cadence. "Check-ins" defeats the acceptance criteria. The client decides what triggers a check-in and what makes one complete.

The shape of the deliverable doesn't determine whether it's good. The presence of edges does. Quantity, cadence, and acceptance are how edges get specified.

### What passes

- "12 ad variations per month, refreshed weekly in the dashboard, monthly review call walking through CPL trends. Functional acceptance: dashboard reflects current campaign data. Procedural acceptance: monthly review call confirms variations are running and reporting is accurate."
- "Website redesign: 5 core pages (home, about, services, contact, blog index) + 6 service-detail pages, delivered to a staging environment by week 6 and migrated to the client's domain by week 8. Functional acceptance: all pages load successfully on the client's domain, pass mobile and desktop usability tests against [defined checklist], forms submit successfully across Chrome, Safari, Firefox. Procedural acceptance: client confirms in writing within 5 business days of go-live."
- "Homepage redesign delivered by week 4. Functional acceptance: page passes the usability checklist. Procedural acceptance: client confirms in writing within 5 business days, or feedback is provided through the revision process."

### What fails

- "Manage your Google Ads." — No quantity, no cadence, no acceptance of either kind. The client interprets this as "everything related to Google Ads forever."
- "Ongoing optimization of conversion rates." — Activity-shaped with no edges. What gets optimized? How often? Optimized to what target?
- "Provide marketing support as needed." — "As needed" is the canonical unbounded clause. Always a flag.
- "Website delivered when client approves." — Procedural acceptance only. No functional bar means the client can withhold approval indefinitely without naming what's wrong.

### What the specialist flags

- Any deliverable missing one or more of quantity, cadence, functional acceptance, procedural acceptance.
- Activity-shaped deliverables where the activity itself has no defined completion state.
- Deliverables that depend on undefined inputs ("we'll deliver X once Y is provided") without specifying what counts as Y being provided.
- Deliverables with procedural acceptance but no functional acceptance — sign-off rituals attached to vague work.

---

## The three-tier revision taxonomy

"Includes 2 rounds of revisions" is the canonical broken revision policy. The fix is a taxonomy that distinguishes three categories of change requests, each with its own handling.

### Refinement

A change to existing pages or design elements within the original direction. The thing exists; the client is tuning it.

Examples: changing a headline, swapping an image, adjusting button color, tightening copy, modifying spacing.

**SOW handling:** Two rounds of refinement included per page. Refinements are batched — the client submits all refinement requests for a given page at once, the agency implements them in a single pass, then delivers. The round count protects the agency from infinite tuning. The batching protects the agency from drip-fed changes that turn one round into five.

### Revision

A structural change to the layout, format, or functionality of an approved page or element. The thing exists, but the spec is changing.

Examples: changing a 3-section homepage layout to 4 sections, restructuring the navigation, adding a feature to an existing page, changing the form fields collected.

**SOW handling:** Two rounds of revision included across the project (not per page — revisions are bigger and rarer). Beyond that, billed at a stated rate.

A global element change — "make all buttons bigger," "change the navigation across the site" — counts as one revision, even when it touches multiple pages. Counting per-page would penalize the client for the agency's choice to use shared components.

### New request

Work not in the original scope. New pages, new sections, new element types, new integrations.

Examples: adding a blog when the original scope didn't include one, adding a Spanish version of the site, adding a booking flow.

**SOW handling:** Always a change order. Never absorbed as a "revision." This is the line that protects the project from scope creep.

### The cumulative trigger

The dangerous case is the redesign-in-disguise: enough refinements stacked together that the page has effectively been redesigned, but the agency hasn't billed for revision work because each individual change was a refinement.

**SOW language:** "If total refinement requests on a single page exceed [N], we'll discuss whether the original direction needs revisiting as a paid revision round."

The number can be 8, 10, 15 — depends on the engagement. The point is that the clause exists. Without it, the agency does four free redesigns and resents the client.

### What the specialist flags

- Revision count without taxonomy distinguishing refinement, revision, and new request.
- Revision count without a cumulative trigger clause.
- "Revisions" defined to include "refinements" with no separate refinement allowance, collapsing the protection.
- New pages, sections, or features being treated as "revisions" in the SOW language.
- Per-page revision counts at all — revisions should be project-wide. Per-page counting penalizes the client for shared components and creates accounting friction over global element changes that should obviously count once.

---

## Approval window mechanics

Without a defined approval mechanism, the project either stalls indefinitely (waiting for client sign-off) or ships against unstated objections (because the agency had to move forward).

The mechanism has four components.

### Named contact

The SOW specifies who has approval authority. One person, by name and role.

This is the harder rule than it sounds. It prevents the spouse-from-nowhere problem in week 6, the franchisor weighing in mid-build, the brother-in-law with strong opinions. The named contact's approval is final; other voices are advisory.

For SMB home services specifically, this often pushes back on the client's own organizational reality — the spouse may genuinely be a partner. The fix is naming both decision-makers if both have authority, not pretending one of them doesn't exist. What the specialist refuses to accept is silence on the question.

### Defined window

Each approval point has a fixed review window. The default the specialist treats as reasonable: 5 business days.

- Within the window: client reviews, approves, or provides feedback in writing.
- On day 5 with no response: the agency sends a final notice — "You have until end of day 6. If we don't hear from you, we'll proceed to the next phase per the timeline in this SOW."
- On day 6 end-of-day with still no response: the agency proceeds.

This is the load-bearing mechanism. Without the day-6 cutoff, the project dies in a black hole. With it, the client has a clear deadline, a warning, and the agency has documented permission to move forward.

### Partial feedback

The most common real-world case isn't the missed window — it's partial feedback. The client says "most of this looks good, we'll send notes on the contact form next week."

Without a rule, the agency is back in the black hole: feedback was received, so the day-6 cutoff doesn't apply, so the project waits indefinitely for the missing notes.

**The rule:** Partial feedback resets the window for the items still under review, but doesn't extend it indefinitely. The same 5-day clock applies to outstanding items, with the same day-6 final notice mechanism. Items the client did not specifically flag are treated as approved within the original window.

This protects both sides. The client gets time on the items they're actually deliberating about. The agency doesn't lose the protection of the cutoff just because the client said "good but I have more notes."

### Written objection only

The SOW specifies that approvals and objections must be in writing — typically email to a specified address. Not text, not phone, not "we mentioned it on the last call."

This isn't bureaucracy. It's evidence. When the client says in month four "we never approved that," the email trail settles it.

### What the specialist flags

- No named approval contact specified anywhere in the SOW.
- No defined approval window for milestones requiring client sign-off.
- No mechanism for what happens when the window is missed.
- No rule for handling partial feedback (the most common real-world case).
- Approvals accepted via any channel without a written-record requirement.

---

## Universal ownership categories

Every SOW must explicitly assign ownership of the assets and accounts the engagement touches. The default — silence — defaults ownership to whoever holds the credentials, which is usually the agency. That's the trap.

The categories vary by engagement, but the universal list:

- **Domain registrar account** — who owns the domain registration, who pays the renewal, who holds the registrar login.
- **Hosting account** — who owns the hosting, whose payment method is on file, what happens at end of engagement.
- **Marketing ops platform account** — for any platform the agency configures (CRM, automation tool, marketing platform). The client should own the workspace or sub-account; if the agency owns it during the engagement, the SOW must specify the transfer mechanism.
- **Ad accounts** — Google Ads, Meta, etc. The client should own the ad account; if the agency runs ads under its own MCC or Business Manager, the SOW must specify how data and access transfer.
- **Analytics and tracking** — Google Analytics property ownership, tag manager containers, conversion tracking accounts.
- **Source files and design assets** — final design files, source code, brand assets. Default: client owns the deliverables; the SOW specifies what gets handed over and in what format.
- **Content** — copy, images, documentation produced during the engagement.

### The walk-away test

For every account category in the SOW, ask: if the engagement ended tomorrow with no notice, what would the client need to do to take over operations? If the answer involves negotiating with the agency for access, credentials, or data, the SOW failed.

The right answer: the client already has the access, already owns the accounts, already holds the credentials, and the agency walking away changes nothing about their operational continuity.

(Specific clause language and the failure modes specific to each account type live in `pricing-and-ownership.md`. This file establishes the universal categories and the test.)

### What the specialist flags

- Silence on any account category that the engagement clearly touches.
- "Agency will provide access" without specifying the access pathway or transfer trigger.
- Hosting or platform accounts under the agency's master account with no transfer clause specifying when and how ownership transfers.
- Ad accounts under the agency's MCC or Business Manager with no clause specifying data and access transfer at end of engagement.
- End-of-engagement transition language without defined timelines and deliverables.
