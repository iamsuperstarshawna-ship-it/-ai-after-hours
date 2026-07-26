# AIVA — Meta Ads Manager Setup Checklist (click-by-click)

_Follow this top to bottom tomorrow. It reflects every current decision. Where a
choice is still open, it's marked ◻ DECIDE. See `aiva-ads-status.md` for full context._

---

## §0 — DECIDE FIRST: how the 3 variants are structured

**The problem:** V1 & V3 send clicks to your **landing page** (website), but V2 uses an
**Instant Form** (on-Facebook lead). In a Leads campaign, **one ad set = one conversion
location.** You can't put website ads and an Instant Form ad in the same ad set and have
them optimize correctly.

Two clean ways to fix it:

### ✅ Option A (RECOMMENDED) — send all 3 to the landing page
- One ad set, one conversion location (Website), all 3 videos as ad units.
- Put the **lead form + TCPA consent checkbox ON the landing page** instead of using
  Meta's Instant Form. You keep the exact same consent/compliance — the checkbox just
  lives on your page.
- **Why:** your budget is only $20–30/day. One consolidated ad set optimizes far better
  than splitting tiny budgets. Simplest to build, cleanest data, no structural conflict.
- Trade-off: on-page forms convert a bit lower than Meta Instant Forms, but with this
  budget, consolidation wins.

### Option B — two ad sets
- Ad set 1 = "Website" conversion location → V1 + V3 (landing page).
- Ad set 2 = "Instant forms" conversion location → V2 (Meta lead form + TCPA consent).
- **Why not (usually):** $20–30/day split two ways ≈ $10–15 each — likely too thin for
  Meta's Leads optimization to exit the learning phase. Only do this if you specifically
  want to A/B the Instant Form flow against the landing page.

**◻ DECIDE:** A or B. If unsure, go **A**. The rest of this checklist assumes **A** and
notes where B differs.

---

## §1 — Campaign level

1. Ads Manager → **Create** → Objective: **Leads** → Continue.
2. Campaign name: **`AIVA — Contractor Launch`**
3. **Advantage campaign budget:** ON. Set **$25/day** (mid of your $20–30 range).
   - _(This puts budget at the campaign level so Meta distributes across ads. If you'd
      rather control it at the ad-set level, leave this OFF and set the budget in §2.)_
4. Special Ad Categories: **None** (contractor services is not a special category).
5. A/B test toggle: **OFF**.

---

## §2 — Ad set level ("Contractor Test")

1. Ad set name: **`Contractor Test — V1/V2/V3`** (Option A) — all three live here.
2. **Conversion location:**
   - Option A → **Website** (you'll paste the landing page URL at the ad level).
   - Option B → this ad set = **Website** for V1/V3; make a 2nd ad set = **Instant forms** for V2.
3. **Performance goal:** Maximize number of leads (default). No cost cap yet.
4. **Budget** (only if campaign budget in §1 is OFF): **$25/day**, ad set level.
5. **Audience — go BROAD:**
   - **Advantage+ audience: ON.** Leave the audience suggestions **empty** or add just
     1–2 loose interests (e.g. *Small business owners*) as hints only.
   - **Do NOT** rely on manual job-title targeting — it's largely non-functional now and
     Meta treats it as a suggestion. The creative does the qualifying.
   - **Location:** your target geo (◻ set your states/metros; US-wide if unsure).
   - **Age:** 30–65+.  **Languages:** English.
6. **Placements: Advantage+ placements (automatic).** Don't hand-pick.
7. ⚠️ **Dynamic Creative: OFF.** Confirm it's off so V1/V2/V3 run as **intact ad units**,
   not auto-remixed. (If the toggle is greyed on, you may have to recreate the ad set —
   Dynamic Creative can't always be switched off in place.)

---

## §3 — The three ad units

For **each** video, create an ad in the ad set:

### V1 — "Never Miss Another Job Call"
- Format: Single video → upload the **final V1 file** (⚠️ confirm brown/cream palette, not gold).
- Primary text (paste):
  > Every missed call is a missed job. 📞 While you're on the job, the phone keeps
  > ringing — and those callers dial the next contractor. **AIVA**, your AI employee,
  > answers every time, 24/7, and books the job. Don't take our word for it — call Ava
  > right now and hear it for yourself: **470-800-9501.**
- Headline: **Never miss another job call**
- Destination: **Website** → landing page URL ◻
- CTA button: **Learn More** _(or Call Now if your page is set up for it; leaving to Ads Manager per current decision)_

### V2 — "Your New Employee Never Sleeps"  (the lead-form variant)
- Format: Single video → upload **final V2 file**.
- Primary text (paste):
  > Thinking about hiring a receptionist? **AIVA**, your AI employee, does the job for a
  > fraction of the cost — answering every call 24/7, booking appointments, and never
  > taking a day off. Plans start at **$199/mo**. See how she'd work for your business 👇
- Headline: **Your new employee never sleeps**
- Destination:
  - Option A → **Website** landing page (form lives on the page).
  - Option B → **Instant Form** (build it per §4).
- CTA button: **Sign Up** or **Get Quote**.

### V3 — "Sounds Human. Works Like Magic."
- Format: Single video → upload **final V3 file** (⚠️ confirm palette).
- Primary text (paste):
  > Worried an AI employee answering your phone will sound cheap or robotic? It won't.
  > **AIVA** sounds human, works like magic, and never misses a call — 24/7. Hear her
  > yourself: **470-800-9501.**
- Headline: **Sounds human. Works like magic.**
- Destination: **Website** → landing page URL ◻
- CTA button: **Learn More.**

---

## §4 — TCPA consent (required wherever V2's lead is captured)

Whether the lead is captured on the **landing page form** (Option A) or a **Meta Instant
Form** (Option B), it MUST include a **checked-by-the-user consent box**. Do **not**
pre-check it.

**Consent checkbox label (paste this):**
> ☐ I agree to be contacted by AIVA / AIVA Virtual Intelligence at the phone number I
> provided, including by an AI voice and automated/pre-recorded calls and texts, for
> the purpose of a demo and follow-up about this service. Consent is not a condition of
> purchase. Message and data rates may apply. I can opt out at any time by replying STOP.

**Also required by Meta on any lead form:** a **Privacy Policy URL.**
**[NEEDS FROM YOU]** the privacy policy URL — or tell me and I'll draft a simple one to host.

> ⚠️ Compliance is real here: that consent is the legal basis for AIVA to call the lead.
> No consent → no AI-voice follow-up call. Never call scraped/cold lists.

---

## §5 — Before you hit Publish

- [ ] Dynamic Creative confirmed **OFF**.
- [ ] All 3 videos are the **final brown/cream** cuts (no leftover gold).
- [ ] Landing page URL is live and shows "Call AIVA / 470-800-9501" clearly.
- [ ] V2's capture point has the **TCPA consent checkbox** + privacy policy URL.
- [ ] Budget set once ($25/day), **not** per ad.
- [ ] Advantage+ audience ON, placements automatic.
- [ ] Payment method active (restriction resolved ✅).

## §6 — After launch
- [ ] **Don't edit for 5–7 days** (learning phase). Daily edits reset it.
- [ ] **[HANDOFF]** wire V2 leads → HubSpot (native FB Lead Ads integration or Zapier).
- [ ] Day 7: I'll review cost-per-lead, best variant, best-performing hook, next test.
