# PostHog Release Notes

*Sample portfolio piece. Feature areas are inspired by PostHog's real product surface (feature flags, data warehouse, Slack integration) but the specific releases, dates, and wording below are written for demonstration purposes.*

---

## v2.14.0 — March 3, 2026

### New features

**Expanded string matching for feature flags**
Feature flag conditions now support "starts with," "does not start with," "ends with," and "does not end with" operators, in addition to the existing exact match and contains options. All string comparisons are case insensitive by default.

This is useful for targeting by patterns rather than fixed values, for example rolling out a flag to every user whose email domain ends with `.edu`, or excluding session IDs that start with a known test prefix.

To use it, open a flag's release conditions, select a property, and choose the new operator from the condition dropdown. No changes are needed for existing flags built on the older operators.

### Improvements

- Flag payload previews now render nested JSON values before rollout, so you can confirm the exact payload a user segment will receive without saving the flag first.
- The flags list page loads faster for organizations with more than 500 flags.

### Bug fixes

- Fixed an issue where duplicate flag names were silently allowed when created through the API, even though the UI blocked them.

---

## v2.15.0 — April 21, 2026

### Breaking change: Product Tours is being retired

Product Tours will stop working for all versions of PostHog on **September 26, 2026**. After that date, existing tours will no longer display to users, and the Product Tours tab will be removed from the left sidebar.

We built Product Tours to help teams walk new users through onboarding flows. It saw solid adoption, but it sits outside where we are focusing engineering effort right now, and keeping it maintained was pulling attention from work with broader impact across the platform.

**What you need to do:**
- If you have active tours, export any tour content you want to keep before September 26. There is no automated migration path.
- If you use tours for onboarding, we recommend evaluating a dedicated onboarding tool, or building a lightweight equivalent with feature flags and in-app messages.
- API endpoints related to tours will return a deprecation warning starting May 2026 and will be removed entirely alongside the September sunset.

We recognize this is disruptive for teams relying on this feature, and we are sorry for the inconvenience. Reach out to support if you need help planning the transition.

### New features

**PyPI as a data warehouse source**
You can now sync package metadata, release history, and known vulnerabilities for any Python package directly into your data warehouse. This uses PyPI's public JSON API, so setup only requires entering the package names you want to track. Syncs run as full refreshes, since PyPI does not expose a reliable changed-since filter.

### Improvements

- Organization admins can now preview which members would lose access before restricting sign-in to verified email domains, including a warning if the change would lock out the admin making it.

---

## v2.15.4 — May 6, 2026

### Fixes

- Fixed a memory leak in session replay caused by click listeners not being cleared when a survey widget was removed from the DOM while still open.
- Fixed an issue where events added to a queue during an in-progress batch flush were dropped instead of included in the next batch.
- Fixed incorrect TypeScript types on the feature flag SDK methods, where numeric and boolean property values required an unnecessary cast. Evaluation behavior is unchanged; this is a types-only fix.

### Improvements

- The Slack assistant now accepts a model or reasoning-effort change mid-conversation. Switching models no longer resets the thread's context.

---

## Changelog index

| Version | Date | Highlights |
|---|---|---|
| [v2.15.4](#v2154--may-6-2026) | May 6, 2026 | Session replay memory leak fix, SDK type fixes |
| [v2.15.0](#v2150--april-21-2026) | Apr 21, 2026 | Product Tours deprecation, PyPI data warehouse source |
| [v2.14.0](#v2140--march-3-2026) | Mar 3, 2026 | New feature flag string operators |
