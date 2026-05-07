# pricing-and-ownership.md

The trigger-based file for pricing and ownership clauses. Loads when the SOW contains pricing language, ownership language, or both. The frameworks file (`deliverable-language-patterns.md`) named the universal categories and the walk-away test. This file goes deeper on each pricing model and each ownership category — what specifically goes wrong, what the SOW should say.

This file gets technical. The voice rule: every detail stays anchored to what the SOW must specify, not how the underlying technology works. If a section reads like a tutorial, it's drifted out of scope.

---

## Part 1: Pricing model failure modes

Four common pricing structures. Each has a position the specialist holds and a set of specific failure modes the SOW should address.

### Flat fee / fixed price

**Position:** The cleanest pricing model when scope is genuinely fixed. Becomes a trap when scope is fluid and the agency tries to absorb changes without billing for them.

**Failure modes:**

- "All-inclusive" language without a defined scope ceiling. The SOW says "$15,000 all-inclusive for the website project." Six weeks in, the client asks for a blog. Was the blog all-inclusive? The agency either eats the work or has the awkward conversation. The fix is "all-inclusive" being explicitly defined: "This fee covers the deliverables listed in Section X. Work outside Section X is a change order at [rate]."
- Milestone payments without acceptance criteria. The SOW says payment is due at "design completion" without defining what completion means. Either the agency stalls payment by claiming incomplete milestones, or the client withholds payment by claiming design isn't done. The fix is each milestone payment tied to specific functional and procedural acceptance: "Payment due upon client written confirmation that [specific deliverables] meet [specific criteria]."
- Lump-sum payment terms that misalign with the work cadence. 50% upfront / 50% on completion sounds clean but creates leverage problems. If the agency runs over, the final 50% becomes the client's only leverage. If the client delays approval, the agency carries the cost of completed work. The fix is staged payments tied to milestones — though staged payments create their own failure modes, addressed in the next section. Example structure: "30% on signing, 30% on staging delivery, 30% on go-live, 10% on post-launch sign-off (within 30 days of go-live)."

**What the specialist flags:**

- Flat-fee SOWs without defined scope ceilings.
- Milestone payments without milestone-specific acceptance criteria.
- Two-payment structures (50/50, 100% upfront, 100% on completion) that create leverage asymmetry.

### Project-based with milestones

**Position:** Stronger than pure flat-fee when the project has natural phases. Failure modes cluster around milestones that don't have hard edges.

**Failure modes:**

- Milestone definition vagueness. "Design phase complete" is not a milestone. "Approved homepage and 5 interior page wireframes, with client written sign-off" is a milestone. Without specificity, milestones become disputes about whether the milestone was actually reached.
- Milestone-blocking dependencies. The SOW says "design phase begins after client provides brand assets." Client takes 6 weeks to provide assets. Now the agency's timeline has slipped through no fault of its own — but the SOW doesn't say what happens. Does the agency push downstream milestones? Bill for waiting time? Re-scope?
- No defined trigger for skipping a milestone. Sometimes a milestone genuinely doesn't apply (no copy revisions needed because the client provided final copy). The SOW should specify what happens to that milestone's payment — does it shift to the next milestone, get refunded, or stay with the agency as a milestone met by absence of revision?

**SOW clauses to push for:**

- Each milestone defined with specific deliverables, functional acceptance, and procedural acceptance.
- Dependency clauses: "If client-provided inputs are delayed beyond [N] business days from the requested date, downstream milestones shift accordingly. Agency will not absorb timeline impact of client-side delays."
- Milestone-skip mechanism for milestones that become unnecessary.

**What the specialist flags:**

- Milestones defined by phase name only ("design phase complete") without specific deliverables.
- No clauses governing client-side delays.
- Milestone payment timing that creates leverage asymmetry.

### Performance-based

**Position:** Rarely fits SMB home services engagements. The audience-specific reasoning lives in `smb-home-services-context.md` (lead-quality blame games, attribution infrastructure thin). This file addresses what the SOW must contain if performance-based pricing is being used despite the warning.

**Failure modes:**

- Undefined attribution methodology. "Bonus paid when leads increase 30%" without specifying how leads are counted, attributed to the agency's work, or measured against a baseline. Both parties will compute different numbers when the bonus question comes up.
- No baseline establishment. The SOW promises performance against a metric that wasn't measured before work started. The client's "before" number is whatever they remember; the agency's "before" number is whatever's documented. Disagreement guaranteed.
- No confounding-factor acknowledgment. The bonus is tied to a metric (inquiries, conversions, revenue) that depends on factors the agency doesn't control: client's sales process, follow-up speed, market conditions, seasonal variation, other marketing the client is running.
- Asymmetric risk. Performance bonus is upside-only for the client — if performance hits, agency gets bonus; if performance misses, agency gets nothing. The agency carries all the downside risk while the client carries all the upside benefit.

**SOW clauses to push for (if the model is being used at all):**

- Defined attribution methodology: "Leads attributed to agency work are those captured through [specific tracking mechanism] and matching [specific criteria]. Disputes resolved by [specific process]."
- Pre-work baseline: "Performance baseline established as the rolling 6-month average of [metric] prior to engagement start, documented in [appendix or separate doc]."
- Confounding-factor acknowledgment: "Performance metrics may be affected by factors outside agency's control including but not limited to seasonal variation, market conditions, and other marketing activities. Performance review will account for [specific known confounders]."
- Symmetric structure: if performance bonus exists, performance penalty does not. The agency takes upside risk; it does not also take downside.

**What the specialist flags:**

- Any performance-based pricing in SMB home services SOWs without all four clauses (attribution, baseline, confounders, symmetric structure).
- Performance metrics tied to outcomes the agency cannot reasonably influence.
- Performance language without a dispute resolution mechanism.

### Hybrid models

**Position:** Compounds the failure modes of the underlying pricing structures rather than balancing them. The boundary line between the components is where SOWs go silent and disputes start.

In SMB home services specifically, hybrid pricing is often a symptom of unresolved scoping conversations during sales. The agency owner is trying to balance predictable retainer revenue with project upside; the client is simultaneously asking for "all-inclusive" (flat-fee psychology) and "performance-based" (result-oriented psychology). The resulting hybrid satisfies neither psychology and creates boundary-policing problems that wouldn't exist with a cleaner single-model structure. If the hybrid exists because the sales conversation didn't resolve scope, the SOW won't fix it. The specialist's recommendation is sometimes to push back to that prior conversation, not just to revise the SOW.

**Failure modes:**

- Base + performance: ambiguous boundary. The SOW says "$3,000 monthly retainer plus performance bonus." What does the retainer cover? What triggers the bonus? When the client gets the same work in a slow month and a peak month, both sides resent the structure.
- Retainer + project: scope leakage. The SOW says "ongoing retainer covers maintenance, additional projects billed separately." Six months in, what counts as "maintenance" vs. "project" has drifted. The retainer is doing project work uncompensated.
- Mixed-margin trap. Some hybrids have agency margin on platform fees built into the structure (e.g., the retainer includes the platform's monthly fee at a marked-up rate). When the client wants to leave, the SOW often makes this margin invisible — but it's the reason the ownership clauses are restrictive.

**SOW clauses to push for:**

- Component-by-component scope: "Base retainer covers [specific deliverables]. Performance bonus paid for [specific criteria]. Additional project work scoped and billed separately."
- Boundary clauses: "Work that falls outside [specific list] is treated as [project / change order / additional retainer]."
- Disclosure of any pass-through or marked-up costs.

**What the specialist flags:**

- Hybrid pricing without component-by-component scope definition.
- "Retainer plus" structures without defined boundaries.
- Any pricing structure that includes pass-through platform costs without disclosure of the markup.

---

## Part 2: Ownership categories, in depth

Seven categories. Each opens with the specialist's position, the common failure modes, and what proper ownership looks like in SOW language.

### Domain registrar

**Position:** Client owns the registrar account from day one. No exceptions.

**Common failure modes:**

- Agency registers the domain "for the client" using the agency's registrar account. Client never gets the login. Renewal happens silently on the agency's credit card, and the cost gets passed through with margin.
- Agency holds the registrar login as "convenience" — client doesn't know who their registrar is, has never logged in.
- Domain ownership and registrar account ownership conflated. The domain is registered to the client's name, but the agency holds the credentials.

**What proper ownership looks like:**

- Client creates the registrar account in their own name, with their own email and payment method. Agency receives admin access to manage DNS as needed.
- Or: agency assists with initial registration but transfers full ownership and credentials within 5 business days of registration.
- Renewal payment method is the client's, not the agency's. The agency never controls whether the domain renews.

**SOW clause language:**

"Client owns the domain registrar account, including primary credentials and payment method. Agency operates with admin-level access for DNS management. At any point, client may revoke agency's access without penalty."

### Hosting

**Position:** Client should own the hosting account directly when possible. When the agency hosts on its own infrastructure for legitimate reasons (managed WordPress on agency servers, agency-tier CDN), the SOW must specify the migration mechanism.

**Common failure modes:**

- Agency hosts the site on its own reseller account. Client never gets server-level access. Migration at end of engagement is "reasonable transition support" with no defined deliverables.
- Hosting fees are bundled into a monthly retainer with margin built in. Client doesn't know what they'd pay if they hosted directly.
- DNS is on the agency's account separate from hosting. Client controls neither.

**What proper ownership looks like:**

- Default: client creates hosting account directly, agency deploys to it.
- When agency hosts: agency discloses that it's hosting on its own infrastructure, names the underlying provider, and defines a migration deliverable that includes file export, database export, DNS transfer, and a defined window.
- When agency hosts and bundles the fee: agency discloses the markup, or offers a no-bundle option for clients who want hosting at cost.

**SOW clause language:**

"Hosting is provided by [vendor/agency-managed]. Client receives [admin access / deployment access / managed access]. At end of engagement, agency provides full migration support including file export, database export, DNS transfer documentation, and 30 days of post-migration support, delivered within 10 business days of engagement end."

### Marketing ops platforms (CRM, automation, marketing platforms)

**Position:** Client owns the workspace or sub-account from day one. Agency operates with admin access. The "agency partner discount" is not a reason to hold the account — it's a reason to disclose the discount and let the client choose how it flows.

**Common failure modes:**

- Agency creates the client's instance under the agency's master account or partner account. Client never has a directly-billed relationship with the platform. Migration requires the agency's cooperation.
- Agency partner discounts (often 20-40% off platform fees) are captured by the agency without disclosure. Client pays full price; agency pockets the difference.
- Sub-account ownership and platform billing relationship conflated. The sub-account is named for the client, but billing flows through the agency.

**What proper ownership looks like:**

- Client creates the platform account directly, in their own name, with their own billing relationship.
- Or: agency creates the sub-account but transfers ownership (including billing relationship) within a defined window, typically 30 days from setup completion.
- When agency-partner discounts apply: the SOW discloses the discount and offers the client a choice — receive the discount directly via partner code, or let the agency pass through the discount with no markup. Both options eliminate captured margin; the client decides which is operationally simpler.

**SOW clause language:**

"[Platform] account is owned by client, with primary billing relationship between client and [platform vendor]. Agency operates with admin-level access. Where agency-partner discounts are available, client chooses between (a) receiving the discount directly via partner code, or (b) the agency passing through the discount with no markup. Agency's access can be revoked by client at any time without penalty."

### Ad accounts

**Position:** Client owns the ad account. Agency operates under the client's account, not its own. The "agency runs ads under its MCC" pattern is sometimes legitimate (legal jurisdiction reasons, billing aggregation) but always requires an exit mechanism.

**Common failure modes:**

- Agency runs ads under its own MCC (Manager Account) or Business Manager. Client never has a direct relationship with the ad platform. At end of engagement, ad history, audiences, and creative assets are stuck in the agency's account.
- Audience data (custom audiences, lookalike audiences, retargeting pixels) lives in the agency's account. Migration requires rebuilding from scratch.
- Pixel installations on the client's website fire to the agency's pixel ID. End of engagement breaks tracking.

**What proper ownership looks like:**

- Default: client creates the ad account directly. Agency receives admin access.
- When agency runs ads under its MCC for legitimate reasons: SOW specifies what transfers at end of engagement (audiences, creative assets, conversion data, pixel ownership) and on what timeline.
- Pixels installed on client's website are client-owned, regardless of who installed them.

**SOW clause language:**

"Ad accounts are owned by client. Agency operates under client's account with admin access. [If agency MCC applies: At end of engagement, agency transfers all custom audiences, lookalike audiences, creative assets, conversion data, and historical performance data to client's directly-owned account, within 10 business days of engagement end.]"

### Analytics and tracking

**Position:** All analytics properties (Google Analytics, Search Console, tag managers) are client-owned. Historical data is client property and transfers at engagement end.

**Common failure modes:**

- Google Analytics property created under agency's account. Client has no direct access.
- Tag manager container under agency's account. Pixel firing depends on agency's continued operation.
- Search Console verified to agency's email. Client cannot see search performance data.

**What proper ownership looks like:**

- Properties created in client's accounts from day one. Agency receives user-level access.
- When properties are created under the agency's account for setup expedience: transferred to client ownership within 5 business days of property creation.
- Historical data export is a defined deliverable at engagement end.

**SOW clause language:**

"Analytics properties (Google Analytics, Search Console, tag manager, conversion tracking) are owned by client. Agency operates with admin or user-level access as appropriate. At engagement end, agency provides documentation of all configured properties, historical data export, and confirmation that no agency credentials remain attached."

### Source files and design assets

**Position:** Client owns all design files, source code, and brand assets produced during the engagement. Agency does not retain source files as leverage.

**Common failure modes:**

- Agency retains "source files" (PSDs, Figma files, raw design files) as a pressure tactic to retain the client. Client gets only the final deliverable, not the editable assets.
- Code repositories under the agency's GitHub organization. Client has no access.
- "We'll provide source files upon request" with no defined timeline or format.

**What proper ownership looks like:**

- Source files transferred to client at engagement end (or earlier, on request) in standard editable formats.
- Code repositories either created under client's organization from day one, or transferred at engagement end.
- "Final deliverables" defined to include source files, not just the rendered output.

**SOW clause language:**

"Final deliverables include both rendered output and editable source files in [specified formats]. Source files transferred to client within 10 business days of engagement end (or earlier on written request). Code repositories [created under client's organization / transferred to client's organization at engagement end]."

### Content (copy, images, documentation)

**Position:** Content produced during the engagement is client property. Stock licensing and third-party assets require explicit handling.

**Common failure modes:**

- Copy ownership undefined. When client wants to reuse copy in another context, agency claims ownership.
- Stock images licensed to the agency, not to the client. License terminates with the agency relationship.
- Documentation produced for the client lives in the agency's tools (Notion, Confluence) and isn't exported.

**What proper ownership looks like:**

- All copy, images, and documentation produced for the client are client-owned at the moment of creation.
- Stock images licensed to client directly, or with transferable licensing.
- Documentation exported and delivered to client at engagement end in usable formats (PDF, Markdown, Word).

**SOW clause language:**

"All content produced during the engagement (copy, images, documentation) is owned by client at creation. Stock images and third-party licensed assets are licensed to client directly or with transferable rights. At engagement end, all documentation is exported and delivered in [specified formats]."

---

## Part 3: The agency-as-vendor-margin trap

Some agencies act as resellers — earning margin on hosting, marketing platforms, ad management, or third-party services the client uses. This is fine if disclosed. It becomes a problem when the margin shapes the ownership structure to lock the client in.

**The pattern:**

- Agency holds the platform account because that's how the agency captures the partner discount.
- The retainer fee includes platform costs without disclosure of the agency's margin.
- Ownership transfer at engagement end means the client loses the discount — which the agency uses as leverage to retain the client even when fit is poor.

**The position:**

The specialist is not against reseller margins. Agencies provide value (vendor management, consolidated billing, expertise) and earning margin for that value is legitimate. The specialist is against reseller margins that are structured to make ownership transfer impossible or expensive for the client.

**What the SOW should specify:**

- **Disclosure.** The SOW names any reseller relationships and the structure of agency margin (markup percentage, partner discount captured, bundled rate vs. cost-plus).
- **Exit path.** The SOW defines what the client pays if they want to terminate the reseller relationship and own the account directly. The exit path should not be punitive.
- **Optional pass-through.** Where partner discounts apply, the SOW offers the client a choice — receive the discount directly via partner code, or let the agency pass through the discount with no markup. Both options eliminate captured margin; the client decides which is operationally simpler.

**What the specialist flags:**

- Reseller relationships not disclosed in the SOW.
- Bundled platform fees without disclosed markup.
- Termination clauses that include "loss of partner pricing" as a penalty for the client.
- Ownership structures where the agency's margin depends on the client not owning the account directly.

---

## Glossary (for non-technical readers)

- **MCC (Manager Account)** — Google Ads' agency-level account that contains multiple client ad accounts. The agency can manage many clients from one MCC.
- **Business Manager** — Meta's equivalent of MCC for Facebook and Instagram ads.
- **Sub-account** — A child account inside a master/partner account. Common in CRMs and marketing platforms. The sub-account is named for the client; ownership of the sub-account vs. the master is a critical SOW distinction.
- **Reseller** — A relationship where the agency buys services (hosting, platform licenses) from a vendor at a wholesale rate and bills the client at a retail rate. The difference is the agency's margin.
- **Partner discount** — A discount offered by platforms to agencies for bringing clients to the platform. Often 20-40%. The discount can flow to the client (cost savings) or be captured by the agency (margin).
