# Canada Post (canada-post)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Canada Post is the primary postal operator in Canada, offering a developer platform with REST and SOAP web services for e-commerce merchants and solution providers. APIs cover shipping label generation, rate calculation, parcel tracking, address validation (AddressComplete), parcel pickup scheduling, returns management, post office location lookup, and service information.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/canada-post/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/canada-post/refs/heads/main/apis.yml)

## Scope

- **Type:** Index
- **Position:** Consumer
- **Access:** 3rd-Party

## Tags

- Address Validation
- E-Commerce
- Labels
- Logistics
- Pickup
- Postal
- Rating
- Returns
- Shipping
- Tracking

## Timestamps

- **Created:** 2026-06-13
- **Modified:** 2026-06-13

## APIs

### Canada Post Rating Web Service

Returns available shipping services and their rates for a given origin postal code, destination, parcel weight, and dimensions. Supports domestic, US, and international destinations. Returns base cost, taxes, transit time, and expected delivery date for each eligible service. Rate calls do not incur charges.

- **Human URL:** [https://www.canadapost-postescanada.ca/info/mc/business/productsservices/developers/services/rating/getrates/default.jsf](https://www.canadapost-postescanada.ca/info/mc/business/productsservices/developers/services/rating/getrates/default.jsf)
- **Base URL:** `https://soa-gw.canadapost.ca`

#### Tags

- Rating
- Pricing
- Shipping

#### Properties

- [Documentation](https://www.canadapost-postescanada.ca/info/mc/business/productsservices/developers/services/rating/getrates/default.jsf)
- [Getting Started](https://www.canadapost-postescanada.ca/info/mc/business/productsservices/developers/services/gettingstarted.jsf)

### Canada Post Contract Shipping Web Service

Enables commercial customers with a Canada Post parcel agreement to create domestic and international shipments, generate shipping labels (PDF or ZPL), retrieve shipment pricing, manage shipment groups, transmit manifests for billing, void labels, and request refunds. Requires a valid customer number and contract ID.

- **Human URL:** [https://www.canadapost-postescanada.ca/info/mc/business/productsservices/developers/services/shippingmanifest/default.jsf](https://www.canadapost-postescanada.ca/info/mc/business/productsservices/developers/services/shippingmanifest/default.jsf)
- **Base URL:** `https://soa-gw.canadapost.ca`

#### Tags

- Shipping
- Labels
- Manifests
- Logistics

#### Properties

- [Documentation](https://www.canadapost-postescanada.ca/info/mc/business/productsservices/developers/services/shippingmanifest/default.jsf)

### Canada Post Non-Contract Shipping Web Service

Allows general businesses and VentureOne card holders to create domestic and international shipments and generate labels without a formal Canada Post parcel agreement. Charges are applied to a credit card on file rather than a contract account.

- **Human URL:** [https://www.canadapost-postescanada.ca/info/mc/business/productsservices/developers/services/shippingmanifest/default.jsf](https://www.canadapost-postescanada.ca/info/mc/business/productsservices/developers/services/shippingmanifest/default.jsf)
- **Base URL:** `https://soa-gw.canadapost.ca`

#### Tags

- Shipping
- Labels
- Logistics

#### Properties

- [Documentation](https://www.canadapost-postescanada.ca/info/mc/business/productsservices/developers/services/shippingmanifest/default.jsf)

### Canada Post Tracking Web Service

Provides parcel tracking capabilities using a PIN (Parcel Identification Number), DNC (Delivery Notice Card), or customer reference number. Returns tracking summary (most recent event) or full tracking details (all scan events), and supports retrieval of a delivery confirmation certificate as a PDF artifact.

- **Human URL:** [https://www.canadapost-postescanada.ca/info/mc/business/productsservices/developers/services/tracking/default.jsf](https://www.canadapost-postescanada.ca/info/mc/business/productsservices/developers/services/tracking/default.jsf)
- **Base URL:** `https://soa-gw.canadapost.ca`

#### Tags

- Tracking
- Shipping
- Logistics

#### Properties

- [Documentation](https://www.canadapost-postescanada.ca/info/mc/business/productsservices/developers/services/tracking/default.jsf)

### Canada Post AddressComplete API

Address validation and auto-complete web service backed by Canada Post's authoritative Canadian address database. Implements a two-step Find/Retrieve flow — Find returns up to 8 candidate matches on each keystroke, Retrieve returns the full validated address record. Also supports international addresses at an additional cost per lookup.

- **Human URL:** [https://www.canadapost-postescanada.ca/ac/support/api/](https://www.canadapost-postescanada.ca/ac/support/api/)
- **Base URL:** `https://ws1.postescanada-canadapost.ca`

#### Tags

- Address Validation
- E-Commerce
- Checkout

#### Properties

- [Documentation](https://www.canadapost-postescanada.ca/ac/support/api/)
- [Pricing](https://www.canadapost-postescanada.ca/ac/pricing/)

### Canada Post Pickup Web Service

Enables e-commerce platforms to schedule, modify, retrieve, and cancel on-demand parcel pickups. Supports checking pickup availability and cut-off times by postal code. Pickups can be booked up to 30 days in advance (with parcel agreement) or 5 days in advance (without agreement), and same-day requests must be submitted at least one hour before the desired time.

- **Human URL:** [https://www.canadapost-postescanada.ca/cpc/en/support/kb/business/parcel-pickup/parcel-pickup-api-integration-tips-for-e-commerce.page](https://www.canadapost-postescanada.ca/cpc/en/support/kb/business/parcel-pickup/parcel-pickup-api-integration-tips-for-e-commerce.page)
- **Base URL:** `https://soa-gw.canadapost.ca`

#### Tags

- Pickup
- Shipping
- Logistics

#### Properties

- [Documentation](https://www.canadapost-postescanada.ca/cpc/en/support/kb/business/parcel-pickup/parcel-pickup-api-integration-tips-for-e-commerce.page)

### Canada Post Returns Web Service

Generates return shipping labels for authorized returns (pre-approved by merchant) and open returns (customer-initiated). Supports both REST and SOAP protocols. Return labels are retrievable for up to 5 calendar days after creation.

- **Human URL:** [https://www.canadapost-postescanada.ca/info/mc/business/productsservices/developers/services/default.jsf](https://www.canadapost-postescanada.ca/info/mc/business/productsservices/developers/services/default.jsf)
- **Base URL:** `https://soa-gw.canadapost.ca`

#### Tags

- Returns
- Shipping
- Labels
- E-Commerce

#### Properties

- [Documentation](https://www.canadapost-postescanada.ca/info/mc/business/productsservices/developers/services/default.jsf)

### Canada Post Find a Post Office API

Returns a list of Canada Post retail post office locations near a given postal code or address, including hours of operation and available services. Useful for presenting drop-off locations to customers at checkout.

- **Human URL:** [https://www.canadapost-postescanada.ca/info/mc/business/productsservices/developers/services/default.jsf](https://www.canadapost-postescanada.ca/info/mc/business/productsservices/developers/services/default.jsf)
- **Base URL:** `https://soa-gw.canadapost.ca`

#### Tags

- Locations
- Post Office
- Retail

#### Properties

- [Documentation](https://www.canadapost-postescanada.ca/info/mc/business/productsservices/developers/services/default.jsf)

### Canada Post Deliver to Post Office API

Allows customers to select a post office as the delivery destination instead of a residential or commercial address at checkout. Integrates with the Find a Post Office service to present eligible pickup locations for a given shipment.

- **Human URL:** [https://www.canadapost-postescanada.ca/info/mc/business/productsservices/developers/services/default.jsf](https://www.canadapost-postescanada.ca/info/mc/business/productsservices/developers/services/default.jsf)
- **Base URL:** `https://soa-gw.canadapost.ca`

#### Tags

- Delivery
- Post Office
- E-Commerce

#### Properties

- [Documentation](https://www.canadapost-postescanada.ca/info/mc/business/productsservices/developers/services/default.jsf)

### Canada Post Service Information API

Provides information about scheduled outages and service disruptions to Canada Post web services, enabling applications to surface maintenance windows to developers and end users.

- **Human URL:** [https://www.canadapost-postescanada.ca/info/mc/business/productsservices/developers/services/default.jsf](https://www.canadapost-postescanada.ca/info/mc/business/productsservices/developers/services/default.jsf)
- **Base URL:** `https://soa-gw.canadapost.ca`

#### Tags

- Status
- Outages
- Operations

#### Properties

- [Documentation](https://www.canadapost-postescanada.ca/info/mc/business/productsservices/developers/services/default.jsf)

## Common Properties

- [Website](https://www.canadapost-postescanada.ca/)
- [Developer Portal](https://www.canadapost-postescanada.ca/information/app/drc/home?execution=e1s1)
- [Documentation](https://www.canadapost-postescanada.ca/info/mc/business/productsservices/developers/services/fundamentals.jsf)
- [Getting Started](https://www.canadapost-postescanada.ca/info/mc/business/productsservices/developers/services/gettingstarted.jsf)
- [Catalog](https://www.canadapost-postescanada.ca/info/mc/business/productsservices/developers/services/default.jsf)
- [Sign Up](https://sso-osu.canadapost-postescanada.ca/pfe-pap/en/registration)
- [Login](https://sso-osu.canadapost-postescanada.ca/lfe-cap/en/login)
- [Sandbox](https://ct.soa-gw.canadapost.ca)
- [Forum](https://www.canadapost-postescanada.ca/info/mc/business/productsservices/developers/services/default.jsf)
- [Integrate Page](https://www.canadapost-postescanada.ca/cpc/en/commercial/integrate-apis.page)
- [LinkedIn](https://www.linkedin.com/company/canada-post)
- [Features](undefined)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
