# AIVA Meta Ads — Project Status (Source of Truth)

_Last updated: 2026-07-26. This is the living state of the AIVA Meta ads launch.
Update this doc as decisions change so no context is ever lost between sessions._

> Lane: ads/marketing only — strategy, copy, lead form, creative, landing-page
> messaging, and the Meta→CRM plan. The LiveKit/Railway voice agent, HubSpot
> wiring, and Twilio are handled in other sessions. Handoffs are flagged **[HANDOFF]**.

---

## The offer

**AIVA** — an AI employee that answers every call 24/7, books appointments, and
never misses a job. Built for home-service contractors (HVAC / plumbing / electrical
first).

- Brand name is always written **all-caps "AIVA"** but **pronounced "Ava."**
  (In ad *scripts/voiceover* she's spoken as "Ava"; in *on-screen text* she's "AIVA.")
- **Pricing:** Essentials **$199/mo** · Growth **$349/mo** · Pro **$549/mo**
- **HVAC Founding Client Offer** = matches the Essentials tier exactly ($199/mo).
- **Demo phone number:** **470-800-9501** (calling it reaches AIVA live — our best proof).

---

## The three ad variants (scripted + produced as video via Higgsfield)

| # | Name | Angle / hook | Destination | Notes |
|---|------|--------------|-------------|-------|
| **V1** | Never Miss Another Job Call | Loss-aversion + live-demo hook | **Landing page** | "Every missed call is a missed job… call Ava right now and hear it for yourself." |
| **V2** | Your New Employee Never Sleeps | Staffing-cost displacement | **Instant Form (lead)** | "…does the job for a fraction of the cost." Form has **TCPA consent checkbox**. |
| **V3** | Sounds Human. Works Like Magic. | "Will AI sound robotic?" objection + camera-bump viral hook | **Landing page** | "Worried an AI employee will sound cheap or robotic? It won't…" |

**Creative to verify before upload:**
- Brand color direction shifted mid-project **gold → warm brown/cream**. ⚠️ Double-check
  which final video files match the final palette before uploading — don't ship a gold cut.
- Confirm final MP4s exist and are the correct (latest) versions for V1/V2/V3.

---

## Destination / CTA (latest decision)

- Meta **won't allow a bare phone number as a Call-Now destination**, so **V1 and V3
  route to the landing page** instead of a direct call link.
- The **landing page** carries the "Call AIVA" messaging with **470-800-9501 displayed
  throughout**, so a click-through still drives the same live-demo action.
- **Only V2** uses the separate **Instant Form** lead flow (with TCPA consent).
- CTA button copy / objective for V1 & V3 is being left to Ads Manager setup rather
  than manually forced.

**Landing page:** https://aiva-meta.base44.app (built on Base44)
**Privacy policy:** https://aiva-meta.base44.app/privacy-policy
_Note: this session's network policy blocks base44.app, so I can't audit the page
contents from here — see the landing-page self-check in the setup checklist §4a._

---

## Compliance — TCPA (do not skip)

- **TCPA requires opt-in consent BEFORE an AI voice contacts any cell number.**
- **Cold-calling scraped contractor lists is not legal.** Do not do it.
- V2's **lead-form consent checkbox is what makes follow-up calls compliant** — it's
  not optional decoration, it's the legal basis for calling that lead.
- Draft consent language for the V2 form is in the setup checklist (`aiva-ads-manager-setup-checklist.md`).

---

## Meta Ads Manager — current state

- **Campaign:** "AIVA — Contractor Launch" · **Objective:** Leads
- **Ad set:** "Contractor Test — V1/V2/V3"
- **Budget:** **$20–30/day total across all variants** (not per ad).
- **Targeting decision:** go **broad + Advantage+**, let the **creative qualify the
  audience**. Manual job-title targeting ("HVAC Technician," "Business Owner") is
  largely non-functional — Meta removed many categories in Jan 2026, and for Leads
  campaigns targeting inputs are treated as *suggestions* the algorithm can override.
- **Payment:** ad account had a payment-unsettled restriction — **now resolved/paid.**
- **Dynamic Creative:** found **ON** → must be turned **OFF** so the 3 variants run as
  intact ad units, not auto-remixed pieces.

---

## ⚠️ Structural issue to resolve before building (flagged by ads lane)

The current plan mixes **two different conversion locations in one ad set**: V1/V3 →
website (landing page), V2 → Instant Form. In a Meta **Leads** campaign, **all ads in
one ad set generally share one conversion location** — you can't cleanly have website
destinations and an Instant Form living in the same ad set. See the setup checklist
for the two ways to resolve this and my recommendation. **This needs a decision before go-live.**

---

## What's still needed

1. Resolve the conversion-location structure (see checklist §0). ⬅ decide first
2. Turn Dynamic Creative OFF.
3. Confirm final video files (correct brown/cream palette) for V1/V2/V3.
4. Get the landing page URL for V1/V3 routing.
5. Build the ad set(s) + 3 ad units with correct routing, broad + Advantage+.
6. Add TCPA consent to V2's form (language in checklist).
7. Launch at $20–30/day; hold edits during the learning phase.

**[HANDOFF]** Meta→HubSpot lead sync for V2's leads (native FB Lead Ads integration or
Zapier), so consented leads flow to the CRM for compliant follow-up.
