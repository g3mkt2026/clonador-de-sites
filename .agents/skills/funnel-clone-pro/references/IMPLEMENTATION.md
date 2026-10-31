# V7 Implementation playbook

1. Confirm ownership/authorization, original URL, preferred mode, target locale, and test/deploy boundaries.
2. Explore with a browser tool if available. Inventory all reachable routes, quiz branches, popups, exit intent, waits, checkout, price and variations. Use fictitious test data only where permitted. Never purchase.
3. Capture screenshots and computed styles at mobile (390x844), tablet (768x1024), desktop (1440x900) and any site-specific breakpoints. Record original asset rights and fallback substitutions.
4. Build a state graph and a source-to-target element mapping. Prioritize exact authorized text, typography, colors, spacing, images and behavior.
5. Choose static HTML/CSS/JS when sufficient; if leads, pricing or authentication need server processing, implement documented backend and safe APIs. Avoid exposing secrets.
6. Put editable content, checkout/WhatsApp URLs, offer data, locale strings, pixel IDs and experiment flags in a validated config. Preserve defaults unchanged unless asked.
7. Analytics: consent gate -> load provider SDK -> emit deduplicated events -> validate in test/debug tools. Never fire purchase on click alone; use verified payment confirmation.
8. Experiments: separate variants, stable anonymous assignment, record exposure, verify tracking and fallback, preserve canonical clone.
9. Leads: test validation and failure states; confirm user consent and data retention. Use sandbox endpoints for testing.
10. VSL: test poster, captions, playback restrictions, progress-based CTA, resume and mobile.
11. Offers: verify price and discount server-side, test valid/invalid coupons, multiple currencies if relevant, checkout sandbox and shipping conditions.
12. Run browser E2E tests for every reachable path or documented bounded coverage, screenshot diffs, link scans, accessibility and measured performance checks.
13. Deliver source, static export where possible, flow map, change log, backup/rollback instructions, screenshots, QA report and accessible preview URL when actually available.
14. Obtain explicit approval before production publish. After deployment verify actual URL and activate monitoring only with a configured provider and alerts.

When an integration is unavailable, supply an adapter stub plus exact setup steps and mark it NOT CONFIGURED. Do not claim operational functionality.
