# Sales-Site Backlog

## Current Priority

- Keep all public wording simple enough for a 65+ pragmatic owner.
- Show money, time saved, and payback wherever it helps the decision.
- Route funding and support questions to `digiteekaart.ee`.
- Keep every conversion path measurable in GA4.

## Automatiseerimine.ee

- Improve the repeated-work calculator with clearer examples by business type.
- Add one small case example: "Excelist teavituseni" with rough before/after numbers.
- Local lead form shipped on the quiz result (feat/automatiseerimine-lead-capture): posts to
  `api/subscribe.js` -> AMOS outreach-capture -> Listmonk double opt-in, same proven pattern as
  mikrokvalifikatsioon.ee. Requires `AMOS_TOPIC_CAPTURE_URL` and `AMOS_CAPTURE_TOKEN` set in this
  Vercel project (same ingress/token mkval already uses) before the form works in production —
  without them it fails honestly with a 503, it does not silently drop leads.
- `funnel_automatiseerimine` currently maps to the shared `evk_base` brand_key in AMOS
  (infra/services/outreach-capture/app/service.mjs CAPTURE_SITE_TO_BRAND_KEY), not a dedicated
  "automatiseerimine" brand. Fine for now; flag if this brand needs its own brand_key later for
  CRM segmentation.

## Digitaliseerimine.ee

- Add more examples where old software does not need to be replaced immediately.
- Expand the manual-work cost calculator with an optional "errors per month" field.
- Add a short "tasuvuse näide" section near pricing.

## Digiteekaart.ee

- After Google Ads data arrives, refine the result/CTA section around phone calls and owner-level next steps.
- Add stronger examples of possible support amount, own contribution and missing information.
- Keep official funding facts checked against official sources before publishing.

## Teekaart.ee

- Improve the route selector with a stronger final CTA per route.
- Add a one-page example of "omaniku teekaart" with practical next-step pricing.
- Cross-link route results to the right microsite with UTM parameters.
