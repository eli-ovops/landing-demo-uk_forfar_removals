# Owned-site CRO and presentation audit

URL: https://forfar-removals.co.uk/  
Access date: 2026-08-29  
Method: live Chrome headless capture, then visual inspection. Technical/SEO observations are secondary and are **not** the purchase case.

## Visual evidence

| Viewport | Evidence file | Result |
| --- | --- | --- |
| Desktop 1440 × 900 | `evidence/forfar_desktop_1440x900.png` | PASS — screenshot captured; branded lorry/landscape visible; cookie panel covers lower first viewport. |
| Mobile 390 × 844 | `evidence/forfar_mobile_390x844.png` | PASS — screenshot captured; content is materially horizontally clipped: slogan, telephone/email and quote control extend beyond right edge; hero text also runs beyond viewport; cookie panel covers initial view. |

## Current experience

| Area | Observation | Customer-facing consequence | Static one-page response (recommendation only) |
| --- | --- | --- |
| Hero | Desktop hero has a strong branded lorry image, but leading copy is a long generic invitation to browse rather than move type/area/proof/next step. | A visitor must read rather than instantly identify the offer. | Lead with “Removals & Storage across Angus, Tayside & Fife”, a compact proof line and one quote path. |
| Navigation | Desktop contains numerous service labels and nested categories before a visitor knows which service suits them. | Choice burden at an already stressful decision moment. | Present 2–3 primary routes and group secondary services; preserve full scope in a concise list. |
| Trust | Current page has real evidence (vehicle, years/family-run claims, directory reviews/affiliations), but the first view prioritises generic copy over this proof. | Valuable reassurance is delayed. | Bring verified, attributable proof beside the service proposition without fabricating numbers or badges. |
| CTA | A “GET A QUOTE” control is present on desktop. In the captured mobile state only its left edge/text is visible at the right boundary. | The primary next step is not continuously visible/usable at 390px. | Use a full-width, clearly labelled call/email/quote action that stays inside the viewport. |
| Mobile | Captured 390px layout retains a desktop-width top header and has horizontal overflow/cropping. Cookie layer blocks much of the first interaction. | Users may not see contact details or the primary CTA without horizontal movement/dismissing consent. | Mobile-first stacked identity, one immediate contact action and controlled line lengths. |
| Links / readability | Home HTML exposes live internal service/contact/quote links and a `mailto:` address. The actual form/quote submission was **not** used. | Link existence is not a conversion or deliverability result. | Keep only verified phone/email/approved future contact route; no fake form. |

## Technical boundary

The owned page is WordPress/Elementor-flavoured from publicly served HTML. This is a **technical observation only**, not a reason to pitch a redesign. `squirrel` v0.0.88 completed a bounded fresh surface audit of 20 pages in this research directory; its saved report is `evidence/squirrel_surface_audit.llm.txt` and reports an overall 36/F. Relevant report findings include missing meta descriptions on sampled core pages, no H1 on sampled service/contact/quote pages, duplicate form IDs on the quote page, numerous render-blocking scripts, and missing observed security headers. These scanner results are a diagnostic lead, not independent proof of business harm, compliance breach, or a purchase motive. Live Chrome visual evidence remains the operative basis for the presentation thesis.

No links were clicked to submit a form; no cookie choice was made; no authenticated content was accessed. The cookie layer was recorded as visible rather than judged unlawful.
