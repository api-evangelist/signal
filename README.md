# Signal (signal)

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
