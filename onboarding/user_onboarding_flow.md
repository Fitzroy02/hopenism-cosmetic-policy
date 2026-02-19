# User Onboarding Flow

## Purpose

This document defines the onboarding flow for new users joining the platform. The flow is designed to be simple, clear, and ethical — with no dark patterns, no forced sharing, and no hidden tracking.

The guiding principle throughout is: **We ask. We don't guess.**

---

## Step 1 — Welcome & Purpose

**What the user sees:**

> Welcome to the platform.
>
> This is a space to find charities, causes, and community support that matter to you.
>
> We'll ask you a few questions to get started. You only need to share what you're comfortable with.

**Design notes:**
- No account creation required at this step.
- No data is collected at this step.
- The user is told what the platform is for before anything else happens.

---

## Step 2 — Data Philosophy

**What the user sees:**

> **We ask. We don't guess.**
>
> We don't track what you click, watch what you browse, or build a profile from your behaviour.
>
> We ask you what matters. You tell us. That's it.
>
> You can update your answers at any time, and you can always choose not to answer.

**Design notes:**
- This step is non-interactive — it is a statement of principle, not a form.
- It exists to build trust before any data is requested.
- No "I agree" button. No checkbox. It is information, not a consent gate.

---

## Step 3 — Key Question

**What the user sees:**

> **Which charities or causes matter to you?**
>
> You can choose as many or as few as you like. You can skip this and add them later.

*[ List of cause categories — e.g. homelessness, mental health, environment, food poverty, disability, older people, children and families, etc. ]*

> Or describe in your own words: [ free text field ]

**Design notes:**
- This is the only required interaction — but it is skippable.
- Multi-select, not single-select. Users are not forced to choose one identity.
- Free text option ensures the list does not exclude anyone.
- No inference is drawn from what is not selected.

---

## Step 4 — Optional Enhancements

**What the user sees:**

> **Want to help us show you more relevant results?**
>
> These questions are entirely optional. Skipping them won't affect your experience.

- **Location** — *Why we ask: so we can show you local charities and events.*
  - [ ] Share my location *(approximate area only — not precise GPS)*
  - [ ] I'd rather not

- **Types of support** — *What kind of support are you interested in?*
  - [ ] Volunteering
  - [ ] Donating
  - [ ] Receiving support
  - [ ] Finding information
  - [ ] I'd rather not say

- **Accessibility needs** — *Do you have any accessibility requirements we should be aware of?*
  - [ ] Yes — please ask me more
  - [ ] No
  - [ ] I'd rather not say

**Design notes:**
- All fields in this step are optional with a "I'd rather not" option clearly visible.
- No field is pre-filled or pre-selected.
- Location is approximate only — the platform does not request or store precise GPS coordinates.
- Accessibility data is handled with particular care and is never used for profiling.

---

## Step 5 — Consent Summary

**What the user sees:**

> **Before you start — here's what you've shared with us:**
>
> - Causes you care about: *[list of selected causes, or "None — you can add these later"]*
> - Location: *[area name, or "Not shared"]*
> - Types of support: *[selections, or "Not shared"]*
> - Accessibility needs: *[yes/no/not shared]*
>
> **What we do with this:**
> We use it to show you relevant charities and services. We don't share it with anyone without asking you first. We don't use it for advertising. You can update or delete this at any time from your profile.
>
> **Your data is anonymous by default.** We don't know who you are unless you choose to tell us.
>
> [ Continue ] [ Change my answers ]

**Design notes:**
- This is a summary, not a long legal document.
- The user sees exactly what has been collected before the platform uses it.
- "Change my answers" must return the user to the relevant step — not restart the whole flow.
- No "I accept terms and conditions" gate at this point. Consent was given at each individual step.

---

## Step 6 — Start Using the Platform

**What the user sees:**

> **You're ready.**
>
> Here are some charities and causes that match what you've told us.
>
> *[ Personalised results based on stated preferences ]*
>
> Not what you expected? [ Update your preferences ] [ Start from scratch ]

**Design notes:**
- The user arrives at a useful, relevant view immediately.
- No upsell, no upgrade prompt, no data-sharing nudge on the landing screen.
- "Update your preferences" and "Start from scratch" are always accessible, not buried in settings.

---

## What This Flow Does Not Include

- No pre-ticked opt-in boxes.
- No "free trial" with billing details required.
- No social sign-in that grants third-party access to profile data.
- No progress bar that implies the user "must" complete every step.
- No urgency language ("Complete your profile now!").
- No dark patterns of any kind.

---

## Alignment

This flow aligns with:

- [governance/data_ethics_statement.md](../governance/data_ethics_statement.md) — Consent-first, ask-don't-infer principles.
- [governance/privacy_first_design.md](../governance/privacy_first_design.md) — Anonymity by default, user control, no secondary use.
- [CONSTITUTION.md](../CONSTITUTION.md) — Transparency, fairness, and protection principles.
- [safeguards/consumer_protection_charter.md](../safeguards/consumer_protection_charter.md) — Consumer rights and dignity standards.
