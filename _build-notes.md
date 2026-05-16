# Build notes — Vitality Med Spa (Mesa)

## Aesthetic
Desert wellness. The spa is in Mesa, AZ — palette riffs on the surrounding Sonoran landscape rather than the generic "clinical white" most med-spa sites default to.

- **Palette:** sand (#efe6d6) / clay (#b4593a) / pine (#2f3d31). A muted bone (#f8f3e8) as base. Highlight gold (#f3c98a) only inside the dark pine sections.
- **Fonts:** Instrument Serif (display) + DM Sans (UI). Per BUILD_SPEC suggestion for this slug.
- **Mood:** warm, trustworthy, established — the visual opposite of a flashing browser warning.

## Solving the biggest_failure (expired SSL)
The current site is a browser-blocked WordPress build. The redesign answers it in three places:

1. **Nav** — a green "Secure Site" lock badge sits left of the phone number.
2. **Hero** — overlay "trust card" reads `🔒 100% MD Supervised — Dr. Kristie Blessitt, MD`. The card visually echoes a browser address-bar padlock — the absent thing on the current site.
3. **Footer** — explicit "Secured by valid SSL · HIPAA-aware intake" line.

These are mockup signals (not a literal SSL claim about the demo URL), but they replace the cognitive space where the visitor currently sees a red warning.

## Differentiator placement
Section 2 (immediately after hero) is the dark pine "Weight Loss + HRT" block with five named protocols and the MD-supervision claim. The current vitalitymedspa.com buries this behind a dropdown.

## Assets used (only from asset_urls)
- `hero.png` — Vitality-Hero-2-640x498.png (their CDN, downloaded with `curl -k` due to expired cert)
- `logo.jpg` — cropped-New-2025-Logo-73-348x116.jpg
- `screenshot-2020.png` — held but not used (it's the 6-year-old hero we're replacing)

No stock photos. Service tiles use solid clay/pine gradients (typographic-rest tiles per BUILD_SPEC) rather than fake imagery.

## Video
- Before scene captures a styled mock-up of the actual Chrome `NET::ERR_CERT_DATE_INVALID` interstitial that every visitor sees today — far more visceral than scrolling their normal homepage. Includes a callout: "Every Mesa, AZ patient searching 'medspa near me' sees this screen before they ever reach your homepage."
- After scene is the full 6634-px mockup, scroll-panned. No zoom. Captions: "MD-supervised weight loss up front" / "Trust signals replace SSL warnings" / "On-page booking added."
