### 2026-05-17 11:00:51 — Codex (GPT)
**Task**: Fix Micro Mayhem signup email routing and submitted button state
**Changes**:
- Routed FormSubmit signup emails to `marie@discoverycollective.com` and copied `charles@discoverycollective.com`.
- Changed the submit button to show a clear localized sent state instead of `...`.
- Kept the success message visible after submit and disabled the email field to prevent duplicate submissions.

**Commit**: `fix: show sent state after signup`
**Status**: ✅ Pushed

---
### 2026-05-17 13:47:47 — Codex (GPT)
**Task**: Test the live Micro Mayhem signup form three times and confirm receipt with gogcli
**Changes**:
- No website code changes.
- Submitted the live form three times with `charlesmartinedd@gmail.com`; each request returned HTTP 200 from FormSubmit and showed `SENT`.
- Searched both `marie@discoverycollective.com` and `charles@discoverycollective.com` with gogcli; no signup notifications were found.

**Commit**: `docs: record signup delivery test`
**Status**: ❌ Failed: FormSubmit accepted submissions but delivery was not confirmed in either Discovery Collective inbox

---
