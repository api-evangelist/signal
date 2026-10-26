# Signal (signal)

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

Signal is a privacy-focused messaging platform that provides end-to-end encrypted communication through open-source applications on mobile and desktop. Their developer ecosystem centers around the open-source Signal Protocol, client SDKs, and server infrastructure, enabling developers to study, audit, and integrate secure messaging capabilities. The Signal Protocol is the most widely deployed end-to-end encryption protocol in the world, used by Signal, WhatsApp, Google Messages, and other platforms.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/signal/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/signal/refs/heads/main/apis.yml)

## Scope

- **Position:** Consuming
- **Access:** 3rd-Party

## Tags

- Encryption
- Messaging
- Security
- Cryptography
- Open Source
- Privacy

## Timestamps

- **Created:** 2026-03-20
- **Modified:** 2026-05-19

## APIs

### Signal Protocol Specifications

The Signal Protocol Specifications define the core cryptographic protocols that underpin Signal's end-to-end encrypted messaging. These include the X3DH (Extended Triple Diffie-Hellman) key agreement protocol for establishing shared secrets between parties, the Double Ratchet Algorithm for deriving new encryption keys per message, the PQXDH (Post-Quantum Extended Diffie-Hellman) protocol for quantum-resistant key agreement, and XEdDSA for EdDSA-compatible signature schemes. These specifications are published independently so they can be adopted by other projects beyond Signal itself.

- **Human URL:** [https://signal.org/docs/](https://signal.org/docs/)

#### Tags

- Encryption
- Messaging
- Cryptography
- Security
- Protocols

#### Properties

- [Documentation](https://signal.org/docs/)
- [Postman Collection](collections/signal-server.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/signal-server.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Signal libsignal SDK

The libsignal SDK provides platform-agnostic APIs used by the official Signal clients and server. It implements the Signal Protocol including the Double Ratchet algorithm, as well as other cryptographic primitives such as AES-GCM encryption and zero-knowledge group functionality. The core implementations are written in Rust, with bindings exposed as Java, Swift, and TypeScript libraries.

- **Human URL:** [https://github.com/signalapp/libsignal](https://github.com/signalapp/libsignal)

#### Tags

- SDK
- Encryption
- Cryptography
- Java
- Swift
- TypeScript
- Rust

#### Properties

- [Git Hub](https://github.com/signalapp/libsignal)
- [Documentation](https://github.com/signalapp/libsignal)
- [Postman Collection](collections/signal-server.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/signal-server.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Signal Server

Signal-Server is the open-source server backend that supports the Signal Private Messenger applications on Android, Desktop, and iOS. Built as a Dropwizard application, it provides REST controllers for account management, message delivery, key distribution, and device provisioning, along with gRPC services and WebSocket endpoints for real-time communication. The server handles user registration, encrypted message routing, push notification delivery, and pre-key bundle management.

- **Human URL:** [https://github.com/signalapp/Signal-Server](https://github.com/signalapp/Signal-Server)
- **Base URL:** `https://chat.signal.org`

#### Tags

- Messaging
- Server
- Backend
- Encryption
- Open Source

#### Properties

- [Git Hub](https://github.com/signalapp/Signal-Server)
- [Documentation](https://github.com/signalapp/Signal-Server)
- [OpenAPI](openapi/signal-server-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/signal-server.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/signal-server.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [AsyncAPI](asyncapi/signal-server-asyncapi.yml) — [AsyncAPI Specification](https://www.asyncapi.com/docs/reference/specification/latest)
- [Spectral Rules](rules/signal-rules.yml)
- [Capabilities](capabilities/secure-messaging.yaml)
- [JSON Schema](json-schema/signal-protocol-entities-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON-LD](json-ld/signal-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [Vocabulary](vocabulary/signal-vocabulary.yml)

### Signal Android SDK

Signal-Android is the open-source Android client for the Signal encrypted messaging platform. It provides the full messaging experience including end-to-end encrypted text messages, voice calls, video calls, group chats, and media sharing. The application integrates the libsignal protocol library for cryptographic operations and communicates with the Signal Server for message routing and delivery.

- **Human URL:** [https://github.com/signalapp/Signal-Android](https://github.com/signalapp/Signal-Android)

#### Tags

- Android
- Mobile
- Messaging
- Encryption
- Open Source

#### Properties

- [Git Hub](https://github.com/signalapp/Signal-Android)
- [Documentation](https://github.com/signalapp/Signal-Android)
- [Postman Collection](collections/signal-server.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/signal-server.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Signal iOS SDK

Signal-iOS is the open-source iOS client for the Signal encrypted messaging platform. It delivers end-to-end encrypted messaging, voice calls, video calls, and group communications on iPhone and iPad devices. The application uses the libsignal protocol library for all cryptographic operations and connects to the Signal Server infrastructure for message delivery and synchronization.

- **Human URL:** [https://github.com/signalapp/Signal-iOS](https://github.com/signalapp/Signal-iOS)

#### Tags

- iOS
- Mobile
- Messaging
- Encryption
- Open Source

#### Properties

- [Git Hub](https://github.com/signalapp/Signal-iOS)
- [Documentation](https://github.com/signalapp/Signal-iOS)
- [Postman Collection](collections/signal-server.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/signal-server.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Signal Desktop SDK

Signal-Desktop is the open-source desktop client for the Signal encrypted messaging platform, built with Electron and TypeScript. It provides end-to-end encrypted messaging, voice calls, video calls, and group communications on Windows, macOS, and Linux. The desktop client links to an existing Signal mobile account and synchronizes messages across devices.

- **Human URL:** [https://github.com/signalapp/Signal-Desktop](https://github.com/signalapp/Signal-Desktop)

#### Tags

- Desktop
- Electron
- Messaging
- Encryption
- Open Source

#### Properties

- [Git Hub](https://github.com/signalapp/Signal-Desktop)
- [Documentation](https://github.com/signalapp/Signal-Desktop)
- [Postman Collection](collections/signal-server.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/signal-server.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [LinkedIn](https://www.linkedin.com/company/signal-messenger)
- [Website](https://signal.org/)
- [Documentation](https://signal.org/docs/)
- [Blog](https://signal.org/blog/)
- [Support](https://support.signal.org/)
- [Terms of Service](https://signal.org/legal/)
- [Privacy Policy](https://signal.org/legal/#privacy-policy)
- [Git Hub](https://github.com/signalapp)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
