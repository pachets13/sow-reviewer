# examples.md

Three worked examples showing the reviewer in action across different engagement types. Each example includes the SOW the user pastes in and the diagnostic review the reviewer returns. The third example also shows pushback handling — what happens when the user disagrees with a flag.

---

## Example 1: Web project SOW with the modal failure cluster

A solo agency drafted this SOW for a roofing company website redesign. It's a competent first draft — basic structure is there, payment terms are sensible — but the deliverables, revisions, and approval mechanics have the failure modes most web project SOWs ship with.

### The pasted SOW

```
STATEMENT OF WORK
Website Redesign for Northstar Roofing

Prepared by: [Agency Name]
Date: [Date]
Project Total: $8,500

PROJECT OVERVIEW

[Agency Name] will deliver a complete website redesign and optimization for
Northstar Roofing. The new website will reflect Northstar's brand, improve
the user experience, and drive growth for the business.

DELIVERABLES

- Custom website design and development
- Up to 8 pages including home, about, services, contact, and blog
- Mobile-responsive layout
- SEO best practices implemented throughout
- Contact form integration
- Basic analytics setup
- 2 rounds of revisions included
- Hosting and domain management for the duration of the project

TIMELINE

The project is estimated to take 6-8 weeks from kickoff. Specific milestones
will be discussed at kickoff. We'll work to deliver the project in a timely
manner.

PAYMENT TERMS

- 50% deposit due upon signing ($4,250)
- 50% balance due upon project completion ($4,250)

APPROVAL AND REVISIONS

Client approval is required at key project milestones. Revisions will be
incorporated as needed during the project. Final approval is required before
launch.

OUT OF SCOPE

The following are not included in this SOW: ongoing maintenance, content
writing, photography, paid advertising, social media management.

TERMS

Either party may terminate this engagement with reasonable notice. Upon
termination, the agency will provide standard transition support.
```

### The reviewer's diagnostic

This SOW has the structural bones of a working contract, but the language inside the bones is doing too little of the work. Three patterns are creating most of the risk: vague deliverable language, an unstructured revision and approval mechanism, and ownership silence on hosting and the domain. Below in severity order.

#### Critical flags

**1. Deliverables fail the quantity/cadence/acceptance test on multiple lines.**

The deliverables list reads like a feature list, not a contract. Most lines have no quantity, no cadence, and no acceptance criteria.

- "Custom website design and development" — what does "complete" mean? When is it complete? How is completion verified?
- "Mobile-responsive layout" — responsive across which breakpoints, tested how?
- "SEO best practices implemented throughout" — "best practices" is unverifiable. The agency can't enforce it; the client can't measure it.
- "Basic analytics setup" — basic to whom? Google Analytics property? Conversion tracking? Tag manager?

*Push for:* each deliverable line answers how many, how often (or by when), and how completion is verified. For analytics specifically: name the analytics platform, the specific properties or events being tracked, and the access requirements. If GA4: property configured under client's account with [specific events] enabled, client receives admin access, events verified firing via real-time view. If another platform: equivalent specificity for what's being configured and how completion is verified.

Example revision for the website itself: "5-8 pages built per the wireframes approved in milestone 1, delivered to staging by week 5 and migrated to client's domain by week 7. Acceptance: all pages load successfully, pass mobile and desktop usability tests against [defined checklist], forms submit successfully across Chrome, Safari, Firefox."

**2. Revision policy is a count without a taxonomy.**

"2 rounds of revisions included" is the canonical broken policy. Two rounds of what? When the client asks to swap a hero image (refinement), restructure the services page from 3 sections to 5 (revision), and add a Spanish-language version (new request), all three will be treated as round 1.

*Push for:* the three-tier taxonomy. Refinements (changes within the original direction) get 2 rounds per page, batched. Revisions (structural changes) get 2 rounds across the project; global changes count as one revision regardless of pages touched. New requests (work outside scope) are always change orders. Plus a cumulative trigger: "If total refinement requests on a single page exceed 8, we'll discuss whether the original direction needs revisiting as a paid revision round."

**3. Approval mechanism has no named contact, window, or missed-window mechanism.**

"Client approval is required at key project milestones" is silence on every load-bearing question. Who approves? Within what window? What happens if the window is missed?

This is also where the spouse-from-nowhere problem lives. Roofing companies are often owner-operator businesses where the spouse has real decision authority but isn't on the sales call. If the SOW names only the owner and the spouse weighs in week 6, the project stalls.

*Push for:* named decision-maker(s) by name and role; 5-business-day approval window starting from acknowledged receipt (not delivery — the owner is doing roofing work and may not see a Friday delivery until Monday); day-6 final notice mechanism with the agency proceeding by end of day 6 if no response; written objection only.

#### Significant gaps

**4. Hosting and domain ownership is undefined.**

"Hosting and domain management for the duration of the project" — whose hosting account? Whose domain registrar? What happens at end of engagement?

If the agency hosts on its own reseller account and registers the domain under its own registrar account, the client cannot walk away cleanly. End-of-engagement migration becomes a negotiation rather than a clean handoff.

*Push for:* explicit ownership clauses. Client owns the domain registrar account from day one, with primary credentials and payment method. Hosting is either client-owned directly or agency-managed with a defined migration deliverable (file export, database export, DNS transfer documentation, delivered within 10 business days of engagement end).

**5. Timeline language is non-binding.**

"Estimated to take 6-8 weeks. We'll work to deliver in a timely manner." — "estimated" makes the timeline non-binding. "Timely manner" is unverifiable. If the agency runs over, there's no consequence; if the client expects on-time delivery, there's no commitment.

*Push for:* specific milestone dates from kickoff (week 2: wireframes; week 4: design approval; week 6: staging delivery; week 7: go-live). Plus a dependency clause: "If client-provided inputs (content, images, brand assets) are delayed beyond the requested date, downstream milestones shift accordingly."

**6. Termination language is vague on the substantive questions.**

"Reasonable notice. Standard transition support." — both phrases are unverifiable. What's reasonable? What's standard?

*Push for:* defined notice period (typically 30 days). Specific transition deliverables: source files transferred, hosting migration completed, credentials documentation provided, post-transition support window defined.

#### Minor refinements

**7.** "Drive growth" in the project overview is outcome-conflation language. The agency is not contractually responsible for the client's growth. Move the language to a "project goals" section if it's important to the client, or remove it. Deliverables stay artifact-based.

**8.** Out-of-scope list is short for a web project, and the verbal sales conversation almost certainly covered items that aren't reflected here. Every meaningful verbal commitment from the sales conversation either becomes a deliverable or gets an explicit exclusion. Without explicit exclusions, the client will expect things in month three based on what they remember from the call. Likely missing exclusions for this engagement: re-training of new staff after launch, post-launch SEO content production, integration with third-party tools not specified in scope, ongoing site updates after the post-launch support window. Push for an exclusion list that pre-empts the conversations the verbal sales discussion likely opened.

**9.** Payment terms create leverage asymmetry. 50/50 with the second 50% on completion gives the client all the leverage at the end. Consider staged payments tied to milestones: 30% on signing, 30% on staging delivery, 30% on go-live, 10% on post-launch sign-off (within 30 days).

#### Closing summary

The single highest-priority fix: Rewrite the deliverables section to pass the quantity/cadence/acceptance test on every line. Without that, the rest of the SOW is decorating a contract that doesn't actually commit the agency to specific work — and every other failure compounds with it.

---

## Example 2: Marketing ops SOW with the configuration-vs-process-design problem

A small agency drafted this SOW for an HVAC company's CRM setup and lead-routing automation. The technical scope reads competently — pipelines, automations, integrations are all named — but the SOW has no acknowledgment that configuring the platform requires a defined business process to configure it for. That's where the engagement will go sideways.

### The pasted SOW

```
STATEMENT OF WORK
Marketing Operations Setup for Summit HVAC

Prepared by: [Agency Name]
Date: [Date]
Setup Fee: $4,200
Monthly Retainer: $1,500/month for ongoing optimization and support

PROJECT OVERVIEW

[Agency Name] will configure Summit HVAC's marketing operations stack to
streamline lead capture, routing, and follow-up. The system will be built
in [CRM platform] and integrated with Summit's existing tools to support
sales and customer follow-up workflows.

SETUP DELIVERABLES

We will configure the following over a 4-week setup period:

- Sales pipeline configuration with up to 6 stages
- Lead capture automations from website forms, phone calls, and chat widget
- Lead routing logic to assign new leads to the appropriate sales rep
- Follow-up automation sequences (initial response, nurture, re-engagement)
- Calendar integration for booking estimates
- Two-way SMS configuration for technician communication
- Review request automation post-job completion
- Custom dashboard for tracking pipeline health and lead-source performance
- Integration with Summit's existing accounting platform via API

ONGOING OPTIMIZATION (MONTHLY RETAINER)

The monthly retainer of $1,500 covers ongoing optimization and support,
including:

- Workflow adjustments as business needs evolve
- Performance monitoring and reporting
- Up to 4 hours of support per month
- Quarterly review calls

TRAINING

We will provide a 90-minute training session for Summit's team upon
completion of setup. Additional training available as needed.

PLATFORM ACCESS

Summit will receive admin access to the platform. The agency will manage
the workspace and configurations. Platform fees are billed through the
agency at standard rates.

PAYMENT TERMS

- Setup fee: 50% on signing ($2,100), 50% on completion ($2,100)
- Monthly retainer billed on the 1st of each month, beginning month 2

TERMINATION

Either party may terminate with 30 days written notice. Upon termination,
agency will provide handoff documentation and account access transfer.
```

### The reviewer's diagnostic

This SOW scopes the technical work cleanly. What it doesn't scope — and what marketing ops SOWs almost always fail to scope — is whose sales process is being configured into the platform. The agency knows how to build the pipelines; the question is whose pipelines they are. Two critical flags below center on this gap. The rest is real but secondary.

#### Critical flags

**1. The SOW configures a sales process that has not been documented.**

This is the central failure mode of marketing ops SOWs at this audience tier, and it's hidden inside language that looks like technical scope.

"Sales pipeline configuration with up to 6 stages." Whose 6 stages? The SOW assumes Summit has a documented sales process that maps to 6 pipeline stages. If they do, the SOW should reference the documentation. If they don't, the agency is being asked to design Summit's sales process — which is a different engagement than configuring a CRM, and one most SMB clients can't articulate clearly when asked.

The same problem runs through every other deliverable. "Lead routing logic to assign new leads to the appropriate sales rep." Routing on what criteria? Geographic territory? Lead source? Service type? Round-robin? "Follow-up automation sequences (initial response, nurture, re-engagement)." What's the cadence? What triggers movement between sequences? What's a re-engagement trigger? "Two-way SMS configuration for technician communication." When do techs get pinged? What triggers a tech-to-customer SMS? What's the escalation path if no response? What counts as a tech being "available"? "Custom dashboard for tracking pipeline health." What metrics constitute health for an HVAC business specifically?

Configuring a marketing ops platform is technical work the agency can scope and deliver. Designing the sales process the platform encodes is business work that requires understanding how Summit actually operates — and that's a different deliverable. The SOW must specify which is happening.

*Push for:* the SOW names which of three scenarios applies, and prices accordingly.

- "Client provides documented sales process before setup begins. Agency configures the platform to match the documented process. If client cannot provide documentation, configuration cannot proceed."
- "Agency designs the sales process as a separate discovery engagement, billed at [rate], delivered before setup work begins. Setup work is scoped after process documentation is approved."
- "Hybrid: client provides rough process description, agency refines and documents it as part of week 1 of the engagement, client approves documentation before configuration begins. The refinement work is included in the setup fee, capped at [N hours]."

Without one of these scenarios specified, the agency will end up doing process design uncompensated — interviewing the owner, reverse-engineering current practice, making decisions the owner should be making — and the engagement will overrun on both timeline and margin.

**2. Workspace ownership is structured for agency control, not client ownership.**

"Summit will receive admin access to the platform. The agency will manage the workspace and configurations. Platform fees are billed through the agency at standard rates."

Three problems stacked.

The workspace is owned by the agency, not by Summit. "Admin access" is not ownership — it's permission that can be revoked. If the engagement ends, Summit doesn't have a directly-billed relationship with the platform; they have access to a workspace that lives inside the agency's master account.

"Standard rates" is undisclosed pricing structure. The agency is presumably capturing a partner discount or charging margin on platform fees. The SOW doesn't disclose the markup, doesn't name what the platform's direct rate would be, and doesn't offer Summit a choice.

Termination handoff is "account access transfer" — also undefined. Transfer of what? On what timeline? With what data and configuration export?

*Push for:* workspace ownership clarified, pricing transparency, defined transfer mechanism.

- "[Platform] workspace is owned by Summit, with primary billing relationship between Summit and [platform vendor]. Agency operates with admin-level access. Where agency-partner discounts are available, Summit chooses between (a) receiving the discount directly via partner code, or (b) the agency passing through the discount with no markup."
- "At engagement end, agency provides full workspace transfer including all configurations, automations, contact data, and historical reports, delivered within 10 business days of termination notice."

This is also where the SOW's monthly retainer language ("ongoing optimization") interacts with ownership. If the agency holds the workspace and Summit can't run the system without the agency, the retainer isn't really optional — it's the price of continued access to Summit's own data. That's the lock-in pattern walk-away cleanliness exists to prevent.

#### Significant gaps

**3. Training scope is under-specified for an audience where adoption is the bigger problem.**

"We will provide a 90-minute training session for Summit's team upon completion of setup. Additional training available as needed."

Two problems. First, "Summit's team" — who specifically? The owner? The dispatcher who will actually use the CRM daily? Field techs receiving SMS? The dispatcher and the techs are the load-bearing users, and a single 90-minute session for "the team" almost certainly doesn't cover them with the depth they need.

Second, "additional training available as needed" leaves the adoption-boundary problem undefined. When the dispatcher quits in month four and the new hire needs training, is that included in the retainer? In additional billing? In setup?

*Push for:* training delivered in formats that survive turnover (recorded sessions, written workflow documentation, role-specific video walkthroughs). Specify the roles being trained. Plus an explicit adoption-boundary clause: "Agency provides [specific training deliverables]; ongoing staff usage and adoption is Summit's responsibility. Re-training of new staff is available as a separate engagement at [rate]."

**4. Hybrid pricing structure has no boundary definition.**

"Setup Fee: $4,200. Monthly Retainer: $1,500/month for ongoing optimization and support."

The retainer covers "workflow adjustments as business needs evolve, performance monitoring, up to 4 hours of support, quarterly review calls." The hybrid line is where this breaks: what counts as "workflow adjustments" vs. "new project work"? If Summit decides in month 6 they want to add a new automation sequence for a new service line, is that within the 4 hours? Outside the retainer? A change order?

The 4-hour cap is a quantity, which is good — but it's the only bound on the retainer scope. "Ongoing optimization" beyond those 4 hours has no acceptance criteria.

*Push for:* component-by-component scope definition. The retainer covers (a) [specific deliverables within the 4 hours], (b) [specific monitoring and reporting], (c) [the quarterly review]. Work outside this list is treated as a change order or a new project, scoped and billed separately.

#### Minor refinements

**5.** "Up to 6 stages" hedges the wrong direction. "Up to" gives the client expectation flexibility while pinning the agency to a ceiling. If 6 is right, say 6. If the right number depends on the documented process, this clause should reference the process documentation rather than name a number.

**6.** Termination handoff timeline is undefined. "Upon termination, agency will provide handoff documentation and account access transfer" — within how many business days, with what specific deliverables? The hosting and platform clauses have the same gap and will compound at termination if not addressed.

**7.** "Ongoing Optimization" as a section header signals an open-ended scope frame even when the bullets below are more specific. The bullet list inside the section is bounded (4 hours, quarterly review), but the header sets the client's mental model for what they're buying. Rename to something the bullets actually describe — "Monthly Retainer Scope" or similar. The header should match the scope, not the marketing language.

#### Closing summary

The single highest-priority fix: Specify which of the three configuration-vs-process-design scenarios applies before the SOW is signed. Without that, the agency is committing to work that depends on inputs the client hasn't been asked to provide, and the engagement will overrun before the technical work even begins.

---

## Example 3: Maintenance retainer SOW with audience-lens failures

This SOW would pass a generic review. It has clean structure, sensible pricing, and reasonable scope. The failures are in what it assumes about how this relationship operates over twelve months — and those assumptions don't survive the operational realities of SMB home services.

### The pasted SOW

```
STATEMENT OF WORK
Maintenance Retainer for Cardinal HVAC

Prepared by: [Agency Name]
Date: [Date]
Monthly Retainer: $1,200/month
Term: 12 months from start date

OVERVIEW

This retainer continues the working relationship established during
Cardinal HVAC's website redesign and CRM setup engagement (completed
March 2026). The retainer provides ongoing support to keep Cardinal's
digital systems running smoothly and continuing to support business
growth.

MONTHLY DELIVERABLES

Each month, the agency will provide:

- 4 hours of website maintenance (content updates, plugin updates,
  security patches, performance monitoring)
- 2 hours of CRM and automation maintenance (workflow adjustments,
  integration monitoring, troubleshooting)
- 1 monthly performance report (traffic, conversion, lead source data)
- 1 monthly check-in call (30 minutes)
- Email support during business hours (Mon-Fri, 9am-5pm CST)

ADDITIONAL SERVICES

Work outside the monthly scope is available on a project basis at
$125/hour. Common additional work includes new page builds, automation
expansions, and seasonal campaign setup.

TRAINING

Initial training was provided as part of the original setup engagement.
Refresher training for existing team members is included in the monthly
support hours. Significant new training (new system features, major
workflow changes) is billed as additional services.

PAYMENT TERMS

Monthly retainer billed on the 1st of each month. Net 15 payment terms.
Annual prepayment offered at 5% discount.

TERMINATION

Either party may terminate with 30 days written notice. Upon termination,
the agency will provide handoff documentation including current
configuration, access credentials, and final performance reports.

RENEWAL

This retainer auto-renews on the anniversary date unless either party
provides 30 days written notice of intent not to renew.
```

### The reviewer's diagnostic

This SOW reads cleanly. The hours are quantified, the deliverables are listed, the pricing is sensible, the termination clause is reasonable. A generic SOW reviewer would have nothing to flag. But this is a maintenance retainer for a roofing-and-HVAC business, scoped to run for twelve months across at least two distinct seasonal cycles — and the SOW treats every month as identical. Three flags below in severity order, each centered on operational realities the SOW hasn't accounted for.

#### Critical flags

**1. Uniform monthly cadence in a seasonal business.**

"Each month, the agency will provide: 4 hours of website maintenance, 2 hours of CRM maintenance, 1 monthly report, 1 check-in call."

This is the structural failure. Cardinal's revenue isn't flat across the year — HVAC peaks in summer cooling and winter heating, with shoulder seasons of meaningfully lower activity. The retainer commits to identical work in February (low-activity month, when the agency could be doing strategic work the client has time to engage with) and July (peak month, when the dispatcher is buried in service calls and the owner has no time for a check-in). One of two things will happen: the agency over-delivers in slow months and resents the rate, or the agency under-delivers in peak months and the relationship strains.

The check-in call is the most visible version of this. A 30-minute monthly call is reasonable in February. In July, getting Cardinal's owner on a 30-minute call is going to require multiple reschedules, late-evening slots, or skips. The SOW doesn't acknowledge this — it treats the call as a calendar item, not as a relationship operation that has to fit Cardinal's actual operating reality.

*Push for:* retainer scope structured by quarterly or seasonal blocks, with deliverable mix that flexes. Off-season blocks lean into strategic work (content production, automation refinement, dashboard improvements). Peak-season blocks lean into reactive support (maintenance, troubleshooting, light updates). The total hours per quarter can stay constant; the mix shouldn't.

The check-in cadence specifically should flex with the season — monthly in shoulder seasons, quarterly review calls during peak with shorter written updates between, recognizing that "we'll catch up after the busy season" is the reality the SOW should bake in rather than fight against.

**2. Pause language is missing entirely, and this audience needs both kinds.**

The SOW has no pause clause at all. It has termination, but termination is irreversible — Cardinal cancels and starts over.

For SMB home services specifically, the SOW needs two distinct pause categories. Seasonal pause is structural: a lawn care company that wants to pause from November to February, an HVAC company that wants to drop to a reduced retainer during slow months. This is planned, predictable, and not a sign of relationship trouble. Relational pause is unplanned: cash flow trouble, business changes, the client needs breathing room. This is the case the 6-month limit applies to — past 6 months of relational pause, the relationship has atrophied and re-engaging is harder than starting fresh.

Without language for either, Cardinal's only option when they need flexibility is termination. The agency loses the relationship over a problem that should have been a pause.

*Push for:* explicit pause clauses for both cases. Seasonal pause defined as a separate scheduled category that doesn't count toward any relational atrophy clock. Relational pause defined with the 6-month limit, after which the parties make a mutual decision to re-scope or terminate. Pause means work stops and billing stops in both cases.

#### Significant gaps

**3. Training scope assumes staff continuity that this audience doesn't have.**

"Refresher training for existing team members is included in the monthly support hours. Significant new training (new system features, major workflow changes) is billed as additional services."

Two problems. First, "existing team members" — what happens when the dispatcher quits in month four and Cardinal hires a new one? The new dispatcher isn't an "existing team member" and isn't getting "refresher training" because they have nothing to refresh. They need initial training, which the SOW only covered in the original engagement. Is the new hire's training in scope? Out of scope? Billed as new training?

Second, the SOW conflates "training" with "support hours." Real training (a new dispatcher learning the CRM from scratch) takes more than 6 hours of support time, but it's getting drawn from the maintenance pool — which means actual maintenance gets squeezed when staff turns over.

*Push for:* explicit re-training language as a separate category. "Training of new staff hired after the initial engagement is available as a separate engagement at [rate]; staff training is not drawn from monthly support hours." Without this, every staff turnover becomes a margin loss the SOW didn't anticipate.

#### Minor refinements

**4.** The "supporting business growth" language in the overview is outcome-conflation that will surface later. The overview says the retainer keeps systems "supporting business growth." If Cardinal has a slow quarter — and they will, that's the cycle in this industry — the retainer becomes the visible thing to blame. The agency is contractually responsible for system uptime and maintenance, not for Cardinal's growth. Move growth language out of the overview, or keep it but explicitly separate "what this retainer does" (maintains systems) from "what Cardinal hopes will result" (continued growth).

#### Closing summary

The single highest-priority fix: Restructure the monthly cadence to flex with Cardinal's actual seasonal reality. Without that, the retainer is a contract neither party can honor as written — the agency over-delivers in slow months and under-delivers in peak — and every other flag here gets harder to resolve once the cadence assumption breaks.

---

### Pushback exchange

The user pushes back on the seasonality flag.

> **User:** "I see the seasonality flag, but I want to push back on this one. We've worked with Cardinal for almost a year now. They're not pure installation HVAC — they have a strong service contract base, so their revenue is steadier than typical seasonal HVAC. The uniform monthly cadence has actually worked for them, and they like the predictability. Do we really need to restructure this?"

> **Reviewer:** Fair pushback. If Cardinal has a meaningful service contract base, their revenue curve is genuinely flatter than pure-installation HVAC, and the uniform cadence may fit how they actually operate.
>
> The risk you're accepting by keeping the uniform structure: even with service contracts, peak service-call season (mid-summer cooling failures, mid-winter heating failures) still hits Cardinal's dispatcher and owner harder than shoulder seasons. The 30-minute monthly check-in is the most likely failure point — getting the owner on a call in late July when the phones are ringing is going to require reschedules. If you've been working with Cardinal for a year and this hasn't been a problem, you have data the generic flag doesn't have.
>
> Two specific things to watch even with the uniform structure: (1) if Cardinal expands into new installation work or grows the team, the retainer assumes a cadence that may not fit the new reality — worth a six-month check-in on whether the structure still fits. (2) The check-in call format specifically may need to flex even when the hour total stays constant — written updates with optional calls during peak weeks, scheduled monthly during slower weeks. If the cadence is working for Cardinal specifically, that's a legitimate override. The risk you're accepting is documented above; if it's an acceptable risk for this client, leave the structure as-is.
