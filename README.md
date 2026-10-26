# yaskawa-robotics

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
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Yaskawa / Motoman — industrial robotics, AC servo motors, drives, and motion control.

Yaskawa Electric Corporation (Kitakyushu, Japan) is the world's largest manufacturer of AC servo motors and motion controllers, and one of the most established industrial robotics vendors through its Motoman brand. This api-evangelist profile catalogs Yaskawa's developer-facing surface across four business segments: **Motion Control** (Sigma-X servo motors and SERVOPACK amplifiers), **AC Drives / Inverters** (GA800, U1000, low- and medium-voltage VFDs), **Robotics** (Motoman articulated, SCARA, delta, mini, and collaborative robots on DX200, YRC1000, and YRC1000micro controllers), and **Systems Engineering**.

## Developer Surface

Yaskawa's developer presence is **SDK- and protocol-driven**, not HTTP/REST. There are no public OpenAPI specifications, so this profile intentionally omits a generated `openapi/` directory. The catalog instead points to:

- **[Yaskawa Motoman Developer Portal](https://developer.motoman.com/en/home)** — the central hub for SDK docs, how-tos, and YIP packages.
- **[Yaskawa-Global on GitHub](https://github.com/Yaskawa-Global)** — official open-source repositories.
- **[YMConnect](https://github.com/Yaskawa-Global/YMConnect)** — modern PC-side communication library for controlling Motoman robots from custom applications (C++ 17 and C#).
- **[MotoROS2](https://github.com/Yaskawa-Global/motoros2)** — a native ROS 2 (rcl, rclc, micro-ROS) node running on MotoPlus-compatible controllers; supports ROS 2 Foxy, Galactic, Humble, and Jazzy, up to 8 motion groups, ~100 Hz control.
- **MotoPlus SDK** — on-controller C development for deterministic timing, multi-tasking communication, position/motion data, variables, I/O, jobs, and alarm/error handling.
- **[MotoCom SDK](https://www.motoman.com/en-us/products/software/development/motocom-sdk)** — legacy Windows SDK for status monitoring, I/O exchange, and variable management.
- **[SmartPendantSDK](https://github.com/Yaskawa-Global/SmartPendantSDK)** — Java SDK for extending the Smart Pendant teach interface.
- **[Smart Packager](https://developer.motoman.com/en/yip/smart-packager)** — tooling for building YIP (Yaskawa Innovation Plus) extension packages.

## Profile Contents

- [`apis.yml`](./apis.yml) — APIs.json 0.20 catalog entry for Yaskawa / Motoman.

## Related

- [api-evangelist/figure-robotics](https://github.com/api-evangelist/figure-robotics) — Figure (humanoid robotics).
