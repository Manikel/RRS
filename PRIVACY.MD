# Privacy Policy for Roblox Region Selector

_Last updated: July 2026_

Your privacy is important. This extension (“Roblox Region Selector”) is designed with privacy by default. Below we explain what data is used, how it is used, and your choices.

---

## Information We Use

- **Server Data**: The extension requests Roblox server lists and server details from Roblox’s public APIs to show available servers and determine each server’s region.
- **Approximate Location**: To estimate your ping by distance, the extension may request your **approximate, city-level** location once from a public geo-IP service (ipwho.is), which derives it from your IP address. It is used only for the ping estimate, is **not stored**, and is not shared with anyone else.
- **Latency Tests**: To display estimated ping, the extension sends lightweight, anonymous requests to public test endpoints (Amazon S3 “ping” objects, and Cloudflare endpoints as a fallback). These contain no personal information.
- **Datacenter Dataset**: About once a week the extension downloads a public, anonymous list of Roblox datacenter locations from `data.roseal.live` so new datacenters are recognized without an update. No personal data is sent with this request.
- **Local Storage**: The extension stores your selected region preference, a local cache of server-to-region results (kept up to 12 hours so re-opening a game is instant), and — only if you use the optional paid feature — an anonymous subscription token. All of this stays on your device.

We do **not** collect, store, or transmit:

- Personal identifiers (name, email, address, etc.)
- Account credentials or passwords
- Browsing history
- Payment or card information
- Personal communications

---

## Shared Server-Region Data

To make the extension faster for everyone, the anonymous mapping of **which server belongs to which region** may be sent to our backend service (`api.rrs.codes`) and shared with other users. This data is about game servers only — it contains **no personal information and is not tied to your identity**. It lets a server another user is about to join show its region instantly instead of being re-checked every time.

---

## RRS Plus (Optional Paid Feature)

RRS Plus is an optional subscription that auto-joins your lowest-ping server.

- **Payments are processed entirely by Stripe** on Stripe’s own secure pages. The extension **never sees, handles, or stores your card details**.
- To check whether RRS Plus is active, the extension stores a **random anonymous token** on your device (synced to your browser profile) and sends it to our backend. The token is not linked to your name, email, or any personal identity.
- You can cancel anytime from the extension’s popup (which opens Stripe’s billing portal).

---

## How We Use Data

- To show available Roblox servers and their regions
- To estimate network latency between your device and each region
- To make the extension faster through local caching and shared, anonymous region data
- To provide and manage the optional RRS Plus subscription

Beyond the anonymous server-region data described above, all processing happens locally in your browser.

---

## Sharing of Data

- We do **not** sell your data, and we do not use it for advertising or tracking.
- The only third parties contacted are the services required for functionality: **Roblox** (server APIs), **Amazon AWS / Cloudflare** (anonymous latency tests), **ipwho.is** (approximate location), **data.roseal.live** (datacenter dataset), our own backend **api.rrs.codes** (shared region data + subscription status), and **Stripe** (payments, only if you subscribe).

---

## Permissions

The extension requests only what it needs to function:

- `https://*.roblox.com/*` — Roblox’s public server, join, and thumbnail APIs
- `https://*.amazonaws.com/*` — latency testing to AWS regions
- `storage` — saving your region preference, the local cache, and the anonymous subscription token
- `declarativeNetRequest` — setting the required User-Agent header on one Roblox join endpoint so server regions can be detected

---

## Your Choices

- You can remove the extension at any time via your browser’s extensions page.
- Clearing browser storage removes all cached data and preferences.
- You can cancel RRS Plus at any time from the extension popup; the recurring charge stops with no further action.

---

## Contact

For questions, issues, or feedback, please open an issue on the [GitHub repository](https://github.com/Manikel/) or contact the developer: **Mani Kelidari (man32k)**.

---

© 2026 Mani Kelidari. All rights reserved.
