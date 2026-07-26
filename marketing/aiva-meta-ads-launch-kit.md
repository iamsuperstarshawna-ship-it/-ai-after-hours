# AIVA Meta Ads — Launch Kit v1

**Goal:** Get home-service business owners (HVAC, electrical, plumbing, painting,
roofing, and other trades) into our funnel to hire AIVA — the AI employee who
answers their phones so they never miss a call or a customer.

**Primary funnel:** Meta **Instant Lead Form** (native Facebook/Instagram form).
**Secondary CTA in every ad:** *Call AIVA now and hear her yourself — 470-800-9501.*
Letting a skeptical trades owner talk to the product for 60 seconds is our single
strongest sales asset. Make it easy.

> Scope note: This doc is the ads/marketing lane — strategy, copy, lead form, creative,
> and the Meta→CRM plan. The actual Meta→HubSpot wiring, the voice agent, and CRM
> config are handled in other sessions. Where a handoff is needed, it's flagged
> **[HANDOFF]**.

---

## 1. The core insight (why this ad works)

A home-service owner's worst, most-felt pain is **the missed call = the lost job.**
When they're on a roof, under a sink, or driving between jobs, the phone rings and
goes to voicemail — and that caller just dials the next contractor. Industry-wide,
a large share of inbound service calls go unanswered, and most callers won't leave
a voicemail; they simply call the competitor.

We do not sell "AI." We sell **"you stop losing jobs to voicemail."** AIVA is framed
as *an employee you hire*, not software you configure — that's the emotional hook and
it matches the brand.

**One-line positioning:**
> "AIVA answers every call your business misses — so a $8,000 job never goes to
> voicemail again."

---

## 2. Campaign structure (Meta Ads Manager)

Keep it simple for launch. One campaign, tight testing.

```
Campaign: AIVA — Leads (Objective: Leads / Instant Form)
│
├── Ad Set A — Broad Trades (interest + advantage audience)
│     Budget: $25/day
│     Placements: Advantage+ (auto)
│     Optimization: Leads
│
└── Ad Set B — Job-title / business-owner targeting
      Budget: $25/day
      Placements: Advantage+ (auto)
      Optimization: Leads
```

- **Campaign budget:** Start at **$50/day total** ($1,500/mo). This is the floor that
  gives Meta enough events to optimize. If that's too high, run **one** ad set at
  $25–30/day instead of two.
- **Bid strategy:** Highest volume (default). Don't set a cost cap until you have
  ~50 leads of data.
- **Conversion location:** Instant forms (on-Facebook lead form).
- **Learning phase:** Expect noisy results for the first ~5–7 days / first 50 leads.
  Do **not** turn ads off or edit them daily during learning — it resets it.

### Naming convention (so reporting stays clean)
`AIVA | Leads | [AdSet] | [Audience] | [CreativeName] | [Date]`
e.g. `AIVA | Leads | A | Broad-Trades | MissedCall-Video | 2026-08`

---

## 3. Targeting

**Geo:** Start US-wide, English. If budget is tight, restrict to the states/metros
where you can actually onboard fastest. *(Tell me your priority metros and I'll tighten this.)*

**Age:** 30–65+. Trades owners skew older; don't waste spend on 18–29.

**Ad Set A — Broad Trades (let Meta's algorithm work):**
- Detailed targeting (interests / behaviors): *HVAC, Plumbing, Electrician,
  Roofer, General contractor, Small business owners, Home improvement,
  ServiceTitan, Housecall Pro, Jobber.*
- Turn **Advantage detailed targeting ON** — Meta will expand beyond these when it
  finds cheaper leads.

**Ad Set B — Owner/decision-maker:**
- Layer: *Small business owners* + the trade interests above.
- Behaviors: *Small business owners*, *Facebook Page admins (business)*.

**Exclusions (both sets):**
- Exclude anyone who already submitted the lead form (custom audience — build it
  after first leads come in).
- Exclude existing customers list once you have one. **[HANDOFF: export customer
  emails/phones from HubSpot → upload as a Custom Audience to exclude.]**

**Retargeting (build in Week 2+):**
- Custom Audience: video viewers (25%+/50%+ of any ad video) + form-openers who
  didn't submit. Run a cheap $10/day "You started — finish signing up" retargeting ad.

---

## 4. The Lead Form (Meta Instant Form spec)

Use a **"More Volume"** form (not "Higher Intent") for launch to keep cost-per-lead
low, then A/B a "Higher Intent" version once you know your close rate.

**Form name:** `AIVA — Never Miss a Call`

**Intro / headline screen:**
- **Headline:** Stop losing jobs to voicemail.
- **Description:**
  > AIVA is an AI employee who answers your business phone 24/7 — books jobs,
  > captures every caller, and never takes a day off. Answer a few questions and
  > we'll show you how she'd work for your business. Want to hear her first?
  > Call her right now: **470-800-9501.**

**Questions (keep it to 4 — every extra field lowers completion):**
1. **What's your name?** *(prefill: full name)*
2. **What's the best number to reach you?** *(prefill: phone)*
3. **What type of business do you run?** *(multiple choice — single select)*
   - HVAC
   - Plumbing
   - Electrical
   - Roofing
   - Painting
   - Other home service
4. **About how many calls do you miss in a busy week?** *(multiple choice)*
   - A few (1–5)
   - A lot (6–15)
   - Too many to count (15+)
   - Not sure

*(Email is auto-prefilled by Meta — keep it as a prefilled field so you capture it
without adding friction. Optional 5th field only if you want it: "Business name.")*

**Completion / thank-you screen:**
- **Headline:** You're in — AIVA's got you covered.
- **Description:**
  > We'll reach out shortly. Can't wait? Call AIVA right now and hear exactly how
  > she'd answer your phones: **470-800-9501.**
- **Button:** `Call AIVA now` → tel link `tel:+14708009501`
- **Also set:** website URL button as backup.

**Privacy policy:** Meta requires a privacy policy URL on every lead form.
**[HANDOFF: I need a privacy policy URL. If you don't have one, tell me and I'll
draft a simple one for you to host.]**

---

## 5. Ad copy — 5 variations to test

Each ad = **Primary text** (the caption) + **Headline** (bold line under image) +
**Description** + **CTA button**. Recommended CTA button: **"Sign Up"** or
**"Get Quote"** (test both). All 5 can run under one ad set; kill losers after ~1 week.

Character notes: keep the first line under ~125 characters so it doesn't truncate
before "See more."

---

### Ad 1 — "The Missed Call" (lead with pain) ⭐ start here
**Primary text:**
> Every call you miss is a job your competitor just booked. 📞
>
> You're on the roof. Under the sink. Driving to the next job. The phone rings —
> and goes to voicemail. Most callers won't leave one. They just call the next guy.
>
> Meet **AIVA** — an AI employee who answers your business phone 24/7. She talks to
> every caller, books jobs, and never misses a ring. No sick days. No "I'll call
> them back."
>
> 👉 See how she'd work for your business — takes 30 seconds.
> Or hear her yourself right now: **470-800-9501.**

**Headline:** Never miss another call (or job)
**Description:** AIVA answers your phones 24/7 so you don't lose work to voicemail.
**CTA:** Sign Up

---

### Ad 2 — "Hire AIVA" (employee framing)
**Primary text:**
> What if you could hire an employee who answers every call, works 24/7, and never
> asks for a raise?
>
> That's **AIVA** — the AI employee built for home-service pros. She picks up when
> you can't, talks to your customers like a pro, and makes sure no job slips through
> the cracks.
>
> HVAC, plumbing, electrical, roofing, painting — if your phone rings, AIVA answers.
>
> 👉 Meet your newest employee below.
> Want to interview her first? Call: **470-800-9501.**

**Headline:** Meet AIVA — your 24/7 AI receptionist
**Description:** Answers every call. Books every job. Never takes a day off.
**CTA:** Sign Up

---

### Ad 3 — "The Math" (ROI angle)
**Primary text:**
> One missed call could be a $5,000 job. 💸
>
> Now do the math on a whole week of missed calls.
>
> **AIVA** answers your phone 24/7 so those jobs stop going to voicemail — and stop
> going to your competition. She costs less than a fraction of a receptionist and
> works every hour of every day.
>
> 👉 See how many jobs you could stop losing.
> Hear her live: **470-800-9501.**

**Headline:** How much is a missed call costing you?
**Description:** AIVA captures every caller so no job goes to voicemail.
**CTA:** Learn More

---

### Ad 4 — "Direct / owner-to-owner" (plain talk)
**Primary text:**
> Home-service owners: you can't answer the phone AND do the job at the same time.
>
> So stop trying. **AIVA** answers every call for you — books the appointment, gets
> the details, keeps the customer happy — while you keep working.
>
> She's an AI employee that runs your phones 24/7. Missed calls become booked jobs.
>
> 👉 Tap below to see her in action.
> Or just call her right now: **470-800-9501.**

**Headline:** You do the work. AIVA answers the phone.
**Description:** The AI employee that answers your business calls 24/7.
**CTA:** Sign Up

---

### Ad 5 — "Try it now" (call-first / demo)
**Primary text:**
> Don't take our word for it. **Call AIVA right now: 470-800-9501.** ☎️
>
> Go ahead — she's an AI employee who answers business phones for home-service pros.
> Ask her anything. That's exactly how she'll sound when she's answering YOUR calls
> and booking YOUR jobs 24/7.
>
> When you're ready to put her to work, tap below.

**Headline:** Call AIVA right now and hear for yourself
**Description:** 470-800-9501 — your future AI receptionist is one call away.
**CTA:** Sign Up

---

## 6. Creative direction

You need **3–4 pieces of creative** to start. Priority order: video first (best for
cold trades audiences), then a couple of static images as backup.

### Creative 1 — Hero video (15–20s) ⭐ highest priority
- **Hook (first 3 sec, MUST work with sound off):** big bold text on screen —
  *"Every missed call = a lost job."* over a phone ringing / going to voicemail.
- **Middle:** show the problem (busy tradesperson can't answer) → introduce AIVA
  answering the call, booking the job. Show a clean phone/chat UI or an AIVA avatar.
- **End card:** *"AIVA — the AI employee who answers your phones. Call 470-800-9501."*
- **Format:** 9:16 vertical (Reels/Stories) is the money placement. Also export 1:1
  for feed.
- **Captions:** burned-in, always. 80%+ watch with sound off.

### Creative 2 — Static "missed call" screenshot
- A phone lock screen showing **"4 Missed Calls"** with red bubbles.
- Overlaid text: *"How many jobs did you just lose? AIVA answers every one."*
- Simple, native-looking, thumb-stopping.

### Creative 3 — "Meet AIVA" branded static
- Clean brand card: AIVA name/logo + tagline *"Your 24/7 AI employee. Never miss a
  call."* + the phone number. Professional, trustworthy, trades-friendly colors.

### Creative 4 — Testimonial / before-after (make once you have a customer)
- "Before AIVA I missed 10 calls a week. Now I book them all." Even a text-on-screen
  quote works before you have a filmed testimonial.

**Design rules for all creative:**
- Trades-owner audience — avoid glossy sci-fi "AI robot" imagery. Keep it grounded,
  credible, benefit-first.
- The phone number **470-800-9501** should appear on every end card / static.
- Mobile-first. Big text. High contrast. Assume sound off.

*I can generate the video and static creative in this session (I have image/video
generation tools). Say the word and I'll produce Creative 1–3.*

---

## 7. Meta → CRM (HubSpot) — the plan

Leads captured in a Meta Instant Form are useless if they sit in Ads Manager. They
need to flow to HubSpot within seconds so AIVA / the team can follow up while the
lead is hot.

**Recommended path (cleanest):**
1. Connect the **Facebook Page** to HubSpot's Ads tool, OR
2. Use HubSpot's native **Facebook Lead Ads** integration to auto-sync new leads as
   contacts, OR
3. If native sync isn't available on the plan, use a **Zapier/Make** connector:
   *Facebook Lead Ads → HubSpot: Create/Update Contact.*

**Field mapping (form question → HubSpot property):**
| Lead form question | HubSpot contact property |
|---|---|
| Name | First name / Last name |
| Best number | Phone |
| (prefilled) Email | Email |
| Business type | Custom property: `trade_type` |
| Calls missed per week | Custom property: `missed_calls_volume` |
| Source | Lead source = "Meta Lead Ad — AIVA" |

**[HANDOFF — this is not my lane, hand this to the CRM/integrations session]:**
- Create the two custom HubSpot properties (`trade_type`, `missed_calls_volume`).
- Connect Facebook Lead Ads → HubSpot (native or Zapier) with the mapping above.
- Set up instant-follow-up (AIVA calls/texts the lead, or a task is created) on new
  contact with source = "Meta Lead Ad — AIVA".
- Give me back: confirmation the sync works + a test lead that landed in HubSpot.

Once that's live, I can build lookalike audiences off closed customers and exclude
existing customers from spend.

---

## 8. Launch checklist

- [ ] **[YOU]** Confirm Business Manager, Ad Account, Page, and payment method are set up.
- [ ] **[YOU/HANDOFF]** Privacy policy URL for the lead form (or ask me to draft one).
- [ ] **[ME]** Produce Creative 1–3 (video + statics) — ready on request.
- [ ] **[ME]** Finalize copy (above — done, ready to paste).
- [ ] **[YOU]** Build the Instant Form in Ads Manager from the spec in §4.
- [ ] **[HANDOFF]** Meta→HubSpot sync + custom properties + instant follow-up.
- [ ] **[YOU]** Launch at $50/day, let it run 5–7 days without edits (learning phase).
- [ ] **[ME]** Report on Day 7: cost-per-lead, best ad, best audience, next test.

---

## 9. What "good" looks like (benchmarks to judge Week 1)

These are directional targets for a lead-gen campaign to trades owners; your real
numbers set the baseline.

- **Cost per lead (CPL):** $8–$25 is a healthy starting range for this kind of B2B
  local lead. Above ~$40 → tighten targeting or refresh creative.
- **Form completion rate:** 20%+ of form-opens should submit. Lower → shorten the form.
- **CTR (link):** 1%+ is fine for cold. Below 0.7% → the creative/hook is weak, swap it.
- **What matters most:** not CPL alone — **cost per booked demo / closed customer.**
  That's why the HubSpot handoff matters. Track leads all the way through.

---

## 10. Roadmap after launch (Meta first, then expand)

- **Now:** Meta (Facebook + Instagram) lead ads — this kit.
- **Week 2–3:** Add retargeting (video viewers + form-openers). Add lookalike
  audience once ~50–100 leads/customers exist.
- **Later:** TikTok (short punchy "call this number and talk to an AI receptionist"
  demo content performs well there) and LinkedIn (owner/decision-maker targeting,
  higher-intent, higher cost). I'll build those kits when you're ready.

---

*Prepared by the AIVA Ads/Marketing lane. Next action from me on request: generate
Creative 1–3, draft a privacy policy, or tighten targeting once you give me priority
metros.*
