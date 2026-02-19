# Quarterly User Survey

## Purpose

This document defines the structure of the platform's three-month user update survey. The survey exists so users can keep their stated preferences current without any obligation to do so. It is anonymous by default.

The survey is not a data extraction exercise. It is an invitation.

---

## Survey Structure

### Introduction (shown before any questions)

> **Time for a quick check-in.**
>
> Three months ago, you told us what matters to you. Things change — and that's fine.
>
> This survey has five short questions. It takes about two minutes.
>
> **Your responses are anonymous by default.** If you'd like us to connect your answers to your profile so we can update your recommendations, you can opt in at the end. That step is entirely optional.
>
> [ Start ] [ Remind me later ] [ Skip this time ]

---

### Question 1 — Current Charitable Interests

> **Which charities or causes matter to you right now?**
>
> *Select all that apply, or describe in your own words.*
>
> *[ Multi-select cause categories ]*
>
> Or in your own words: [ free text field ]
>
> [ ] I'd rather not say

---

### Question 2 — Change in Priorities

> **Have your priorities or interests changed since you last updated your profile?**
>
> - [ ] Yes, my interests have shifted
> - [ ] Mostly the same, but a few things have changed
> - [ ] No, my priorities are the same
> - [ ] I'm not sure
> - [ ] I'd rather not say

*If the user selects "Yes" or "Mostly the same but a few things have changed", a follow-up prompt appears:*

> *Would you like to update your cause preferences now?* [ Yes ] [ No, keep as is ]

---

### Question 3 — Type of Support

> **What type of support are you most interested in right now?**
>
> *Select all that apply.*
>
> - [ ] Volunteering opportunities
> - [ ] Ways to donate (money, goods, or time)
> - [ ] Receiving support or services
> - [ ] Finding information or guidance
> - [ ] Connecting with others in my community
> - [ ] I'd rather not say

---

### Question 4 — Barriers to Engagement

> **Have you experienced any barriers to engaging with charities or services on the platform?**
>
> - [ ] No, I haven't had any issues
> - [ ] Yes — I couldn't find what I was looking for
> - [ ] Yes — results weren't relevant to me
> - [ ] Yes — I had an accessibility issue
> - [ ] Yes — something else
> - [ ] I'd rather not say

*If the user selects any "Yes" option, a follow-up prompt appears:*

> *Would you like to tell us more?* [ Open text field — optional ]

**Design notes:**
- Barrier data is used only to improve the platform. It is not linked to individual users unless consent is given.
- Open text responses are reviewed in aggregate, not individually, unless the user has opted in to profile linkage.

---

### Question 5 — Profile Update Preference

> **Would you like to update your profile based on your answers today?**
>
> - [ ] Yes — update my profile with today's answers
> - [ ] No — keep my profile as it is
> - [ ] I'd like to review my profile first [ Takes user to profile view ]

---

### Closing Step — Optional Identity Linkage

> **Your answers have been recorded anonymously.**
>
> If you'd like your responses linked to your profile so your recommendations are updated, you can opt in here.
>
> - [ ] Yes, link my answers to my profile and update my recommendations
> - [ ] No, keep my answers anonymous
>
> *Choosing "No" does not affect your access to the platform or the quality of your experience.*
>
> [ Done ]

---

## What This Survey Does Not Do

- It does not run automatically or silently in the background.
- It does not collect data the user has not explicitly provided in this session.
- It does not use responses to build a behavioural model.
- It does not share responses with third parties.
- It does not penalise users who skip or decline.
- It does not nudge users toward sharing more than they intend to.

---

## Survey Frequency and Delivery

- Offered once every three months to active users.
- Delivered as an in-platform prompt, not by email, unless the user has opted in to email updates.
- Dismissible without penalty at any point.
- Not repeated more than once in any 30-day period if previously dismissed.

---

## Alignment

This survey aligns with:

- [governance/data_ethics_statement.md](../governance/data_ethics_statement.md) — Consent-first, ask-don't-infer principles.
- [governance/privacy_first_design.md](../governance/privacy_first_design.md) — Anonymity by default, user control, no secondary use.
- [onboarding/user_onboarding_flow.md](./user_onboarding_flow.md) — Consistent language and consent patterns.
- [CONSTITUTION.md](../CONSTITUTION.md) — Transparency and protection principles.
