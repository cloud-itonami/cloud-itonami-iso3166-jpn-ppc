# Business Model: Independent PPC Personal-Data Compliance Service — Japan (PPC)

## Classification

- Repository: `cloud-itonami-iso3166-jpn-ppc`
- ISO 3166 (agency-level): `JPN-PPC`, parent `JPN`
- Ooyake cross-reference: `gov.jpn.dataprotection` (Personal Information Protection Commission / 個人情報保護委員会)
- Activity: compliance with the Act on the Protection of Personal Information (個人情報の保護に関する法律/個人情報保護法, APPI) for a government contractor handling citizen personal data, data-breach notification obligations, and cross-border data-transfer restrictions relevant to foreign SaaS vendors
- Social impact: [:citizen-data-protection :cross-border-transfer-clarity :public-spend-transparency]

## Customer

- an IT or data operator handling citizen personal data as part of a government contract
- a foreign SaaS vendor needing to confirm APPI cross-border data-transfer requirements before bidding
- an operator needing a documented data-breach notification procedure for a public-sector data-processing contract

## Offer

- APPI personal-data classification walkthrough for the operator's specific data flows
- cross-border data-transfer compliance checklist
- data-breach notification procedure template
- compliance-audit export package for the operator's own records

## Revenue

- per-engagement compliance-review fee
- recurring regulatory-change monitoring subscription
- compliance-audit export package

## Trust Controls

- any actual filing, registration, or compliance-program submission
  requires Data Protection Compliance Governor clearance and always escalates to human
  sign-off (`:filing/submit` is never automated at any phase)
- a false or fabricated regulatory-requirement claim is a HARD hold that
  cannot be overridden by human approval alone — it must be corrected
  against a cited PPC source first
- this service does **not** provide legal or tax advice; characterization
  and filing on the client's behalf beyond checklist/draft assistance
  routes to Japan-licensed counsel or a registered agent
- every requirement cites the official PPC source or
  regulation, never invented

## Boundary with adjacent actors (read before forking)

- **`cloud-itonami-iso3166-jpn`**: the COUNTRY-level coordinator (general
  Japan public-sector market entry). This repo is a narrower, deeper
  AGENCY-level leaf — most operators need the country-level blueprint plus
  only the agency-level blueprints that actually apply to their contract.
- **`com-etzhayyim-ooyake`** (etzhayyim/root): read-only civic-wayfinding
  mirror of government structure, non-commercial, barred from acting as or
  for the government (G3 impersonation ban). This blueprint is commercial
  and never claims to be Personal Information Protection Commission or an official channel.
- **`matsurigoto`** (etzhayyim/root): sovereign e-government statecraft —
  literally the government. This blueprint is an independent operator that
  engages with PPC under its public rules — never the
  agency itself.
- **`com-etzhayyim-toritsugi`** (etzhayyim/root): guides a consenting
  INDIVIDUAL citizen through their OWN procedure, non-profit,
  donation-only. This blueprint's client is a business operator, not an
  individual citizen, and it is commercial.
- **`cloud-itonami-M6910`**: helps a client BECOME a legal entity
  (incorporation, ISIC 6910) — a prior, different regulatory phase (company
  law). This blueprint assumes incorporation is already done and handles
  PPC-specific compliance (a different regulatory domain).
