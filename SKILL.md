---
name: funnel-clone-pro
description: Reconstruct and validate user-owned sales funnels, quizzes, VSL pages and checkouts with high visual and behavioral fidelity, preview, HTML export, and approval-gated deployment, analytics, experiments, lead capture, security, offer management, and post-launch monitoring.
---
# Funnel Clone Pro V7

## Scope and permissions
Work on sites the user owns or is authorized to reproduce. Preserve exact copy, colors, spacing, responsive behavior, buttons, transitions and branching where source assets and access allow. Do not silently change content. If an original image is unavailable, request it or generate a similar original replacement when an image-generation tool is available, and flag the difference. Never claim exact equivalence without verification.

## Start of every project
Ask for source URL, whether automatic or step-by-step mode, target language (default unchanged), destination links and deployment preference. Request credentials only through approved secure integrations; never ask users to paste secrets into chat or commit them to code.

## Explore before building
With an authorized browser automation tool, inventory every accessible page and state. Click all quiz answers and buttons, test back/forward, explore branches, waits, exit-intent, popups, countdowns, responsive breakpoints, and accessible offers. Record screenshots and state graph. For registration forms, use clearly labeled fictional test identities only where permitted; do not bypass verification, submit real transactions, create paid subscriptions, or trigger live marketing without authorization. Reach checkout and record observed pricing, currencies, bumps, variants and shipping; mark inaccessible post-purchase upsells as unverified. Avoid flooding production endpoints.

## Build
Reproduce user-owned original as closely as feasible: exact text, punctuation, emoji, typography, color, layout, button behavior, quiz logic, VSL placement, animation and responsive design. Translate only when requested. Replace WhatsApp, checkout, analytics and marketing destinations with user-provided ones, never carry over third-party secrets. Include accessibility, performance and basic security checks without changing intended appearance.

## Modes
- Automatic: inventory, implement, test and present preview, pausing for missing essentials or permission-gated actions.
- Step-by-step: inventory and present a page/branch map, then implement each screen for approval before proceeding.

## Visual QA
Capture original and reconstructed screenshots at matching viewports and states. Compare side by side, fix deviations, rerun interactions and report remaining differences and blocked states. Verify mobile, tablet and desktop. Never report tests as passed unless actually run.

## Deliverables and preview
Produce a usable project, README, assets manifest, flow map, test report and export when feasible. For static funnels, supply a portable HTML/CSS/JS build with index.html and assets; when server functionality is needed, document runtime and backend requirements rather than promising a single standalone HTML file. Start a local preview when supported and provide the actual accessible preview URL or instructions. Never fabricate a preview link. Allow iterative user review and corrections before final publication.

## Deployment
Prepare deployment to Vercel, Netlify or user-selected hosting. If authenticated integration and permission are available, offer preview deployment and verify it; request explicit approval before production deployment, domain/DNS changes, purchases or other consequential actions. Provide deployment instructions when direct publishing is unavailable. Verify deployed routes, assets, links and mobile behavior. Keep test checkout in sandbox until production is approved.

## Report
Summarize what was observed, recreated, changed, blocked, tested, and deployed. Identify uncertain prices and inaccessible screens. Distinguish preview from production URL.

## V7 mandatory capabilities
Read `references/IMPLEMENTATION.md` before planning and `references/QA_CHECKLIST.md` before delivering. Use `templates/project-config.example.json` as a model, not as a source of live IDs or credentials. Record every unimplemented capability explicitly; never claim a service is configured merely because code scaffolding exists.

### Analytics and consent
Support Meta Pixel, GA4 and TikTok Pixel using user-supplied identifiers, configured per environment. Maintain a documented event taxonomy (page_view, quiz_start, quiz_step, quiz_complete, lead_submit, view_offer, initiate_checkout, purchase only after verified provider confirmation). Prevent duplicate events; do not fabricate purchases. Respect consent preferences, LGPD and applicable cookie requirements. Test in debug modes and ensure personal information is not included in analytics URLs or event payloads. Never copy original site's pixel IDs.

### A/B experiments
Create versioned variants and deterministic visitor assignment with sticky cohorts and configurable split. Track exposure and conversions by variant; provide sample-size and significance caveats. Do not assert a winning variant without sufficient data. Never change the source clone without approval; experiments live in separate variants.

### SEO and performance
Use semantic markup, titles/descriptions, canonical URL, social preview metadata, sitemap/robots when appropriate; avoid indexing staging and private checkout paths. Optimize assets, lazy loading, layout stability and caching while preserving screenshot fidelity. Report measured metrics only when measured.

### Backup and editing
Keep source snapshots, project version tags, config history and a documented restore process. Exclude secrets and real lead data from backups unless protected and authorized. Centralize editable copy, images, prices, links and offers in validated configuration, without requiring the user to edit source code. Provide a changelog and rollback plan.

### Lead capture
Connect only user-approved CRM, email or WhatsApp services; validate fields, consent, anti-spam, retries, failure handling and test submissions. Avoid sending fictitious records to production CRM without authorization. Store only necessary data, provide retention/deletion controls and secure transport.

### VSL behavior
Map original video controls, muted autoplay constraints, captions, playback progress, resume behavior, delayed CTA reveal and responsive aspect ratio. Use only user-authorized media. Test timed interactions with real playback state; never claim browser autoplay works everywhere.

### Branch coverage
Build a directed graph of quiz states and conditional outcomes; enumerate answer choices and back/forward behavior. For combinatorial explosions, apply bounded pairwise/path coverage, document what was not tested, and prioritize checkout-reaching paths. Validate state persistence, refresh, mobile, and errors.

### Offer management
Make currency, price, product bundles, coupons, shipping rules, order bumps, eligibility and conditional offers configurable. Source final payable amount from the authorized checkout/provider; never invent discounts or represent a test price as live. Prevent client-side price tampering and require server/provider validation.

### Post-launch monitoring
When user approves a monitoring provider, configure uptime and link/route checks, checkout smoke tests in sandbox, alert destination, cadence and escalation. Do not claim continuous monitoring without an actually running service and confirmed alerts. Avoid real orders and excessive traffic.

### Visual quality report
Deliver before/after screenshots at matching viewports, visual diff artifacts if supported, branch coverage, functional test results, accessibility/performance notes, event verification, consent checks, outstanding gaps, preview URL and explicit approval status. Label each item verified / failed / blocked / not tested.

### Publication and approval gate
Generate portable HTML/CSS/JS for static funnels; document backend dependencies where necessary. Preview locally or on a temporary hosting environment if credentials and tools permit. Require explicit user approval for production publishing, DNS changes, paid resources, marketing sends, or real transactions. Never invent URLs.
