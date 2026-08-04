# Lara Networks

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

Lara Networks, Inc. (founded as **Lara Technology, Incorporated**) was a fabless semiconductor company
headquartered at 110 Nortech Parkway, San Jose, California. It architected, designed, and marketed
silicon-based packet-processing solutions for high-speed Internet and networking infrastructure, built on
its patent-pending **Associative Processing Technology (APT)** and manufactured on 0.18-micron process
technology.

Its product portfolio was **Network Database Search Engine (NDSE)** devices, network coprocessors, and
NDSE subsystems, with **Content-Aware Switching (CAS)** solutions in development. These were
content-addressable memory search engines that offloaded ultra-large table lookups from network
processors — holding tables of more than three million addresses and sustaining over 100 million lookups
per second, so switches and routers could process packets from Layer 2 to Layer 7 at full line rate at
OC-48 (2.5Gbps) and above. Parts shipped under the `LTI7000` (Lara Technology) and `LNI7000` (Lara
Networks) family names.

In **October 2000** the company secured a **$40 million second round led by Raza Ventures**, with Battery
Ventures, InveStar Capital, and TeleSoft Venture Partners participating, alongside a long-term
co-development agreement and minority equity investment from **STMicroelectronics**.

## Status: acquired — no API surface

The company no longer operates independently. Verified by live probe and archive review (2026-07-19):

- `https://www.laranetworks.com/` `301` → `https://www.infineon.com/about/company?site=www.laranetworks.com`
- Every path, including `/.well-known/security.txt`, `/.well-known/api-catalog`, and `/llms.txt`,
  301-redirects to the same Infineon corporate page; the `site=` parameter echoes the requested hostname,
  Infineon's standard handling for domains it holds from acquired entities
- `whois laranetworks.com`: created 2000-01-22, registrar **CSC Corporate Domains**, name servers
  `pdns1/pdns2.cscdns.net` — an enterprise corporate registrar, not an expired or parked domain
- The apex `laranetworks.com` does not answer over HTTPS; only the `www` host responds, and only to redirect
- Wayback snapshot **2001-05-15** shows the live Lara Networks site (APT, NDSE, LNI7000) and an investors
  page naming Battery Ventures, InveStar Capital, Raza Ventures, TeleSoft Venture Partners, and STMicroelectronics
- Wayback snapshot of `/aboutus/profile.cfm` serves **"Cypress - About Us"** dated Jan. 16, 2003,
  copyright Cypress Semiconductor Corporation — the domain had been folded into Cypress's site by then
- Cypress Semiconductor was itself **acquired by Infineon Technologies in April 2020**, which is why the
  domain now terminates at infineon.com

As a fabless chip company selling silicon to network equipment manufacturers, Lara Networks never operated
a web or developer API program, so there is nothing to enrich beyond identity and domain posture. The only
artifact in this repo is a live domain-security probe of the redirecting host.

Backed by: battery-ventures
