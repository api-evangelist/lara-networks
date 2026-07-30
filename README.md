# Lara Networks

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
