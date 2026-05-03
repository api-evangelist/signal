# Signal (signal)
Signal is a privacy-focused messaging platform that provides end-to-end encrypted communication through open-source applications on mobile and desktop. Their developer ecosystem centers around the open-source Signal Protocol, client SDKs, and server infrastructure, enabling developers to study, audit, and integrate secure messaging capabilities. The Signal Protocol is the most widely deployed end-to-end encryption protocol in the world, used by Signal, WhatsApp, Google Messages, and other platforms.

**URL:** [Visit APIs.json URL](https://raw.githubusercontent.com/api-evangelist/signal/refs/heads/main/apis.yml)

## Scope

- **Type:** Contract
- **Position:** Consuming
- **Access:** 3rd-Party

## Tags:

 - Encryption, Messaging, Security, Cryptography, Open Source, Privacy

## Timestamps

- **Created:** 2026-03-20
- **Modified:** 2026-05-02

## APIs

### Signal Protocol Specifications
The Signal Protocol Specifications define the core cryptographic protocols that underpin Signal's end-to-end encrypted messaging. These include the X3DH key agreement protocol, the Double Ratchet Algorithm, the PQXDH post-quantum protocol, and XEdDSA signature schemes.

**Human URL:** [https://signal.org/docs/](https://signal.org/docs/)

#### Tags:

 - Encryption, Messaging, Cryptography, Security, Protocols

#### Properties

- [Documentation](https://signal.org/docs/)

### Signal libsignal SDK
The libsignal SDK provides platform-agnostic APIs implementing the Signal Protocol including the Double Ratchet algorithm and cryptographic primitives. Core implementations are in Rust with Java, Swift, and TypeScript bindings.

**Human URL:** [https://github.com/signalapp/libsignal](https://github.com/signalapp/libsignal)

#### Tags:

 - SDK, Encryption, Cryptography, Java, Swift, TypeScript, Rust

#### Properties

- [Documentation](https://github.com/signalapp/libsignal)

### Signal Server
Signal-Server is the open-source server backend supporting Signal Private Messenger applications. Provides REST controllers for account management, message delivery, key distribution, and device provisioning, along with WebSocket endpoints for real-time communication.

**Human URL:** [https://github.com/signalapp/Signal-Server](https://github.com/signalapp/Signal-Server)

**Base URL:** https://chat.signal.org

#### Tags:

 - Messaging, Server, Backend, Encryption, Open Source

#### Properties

- [Documentation](https://github.com/signalapp/Signal-Server)
- [OpenAPI](openapi/signal-server-openapi.yml)
- [AsyncAPI](asyncapi/signal-server-asyncapi.yml)
- [SpectralRules](rules/signal-rules.yml)
- [Capabilities](capabilities/secure-messaging.yaml)
- [JSONSchema](json-schema/signal-protocol-entities-schema.json)
- [JSONLD](json-ld/signal-context.jsonld)
- [Vocabulary](vocabulary/signal-vocabulary.yml)

### Signal Android SDK
Signal-Android is the open-source Android client providing end-to-end encrypted messaging, voice calls, video calls, and media sharing. Integrates libsignal for cryptographic operations.

**Human URL:** [https://github.com/signalapp/Signal-Android](https://github.com/signalapp/Signal-Android)

#### Tags:

 - Android, Mobile, Messaging, Encryption, Open Source

#### Properties

- [Documentation](https://github.com/signalapp/Signal-Android)

### Signal iOS SDK
Signal-iOS is the open-source iOS client for end-to-end encrypted messaging, voice and video calls on iPhone and iPad devices.

**Human URL:** [https://github.com/signalapp/Signal-iOS](https://github.com/signalapp/Signal-iOS)

#### Tags:

 - iOS, Mobile, Messaging, Encryption, Open Source

#### Properties

- [Documentation](https://github.com/signalapp/Signal-iOS)

### Signal Desktop SDK
Signal-Desktop is the open-source Electron desktop client providing end-to-end encrypted messaging on Windows, macOS, and Linux. Built with TypeScript.

**Human URL:** [https://github.com/signalapp/Signal-Desktop](https://github.com/signalapp/Signal-Desktop)

#### Tags:

 - Desktop, Electron, Messaging, Encryption, Open Source

#### Properties

- [Documentation](https://github.com/signalapp/Signal-Desktop)

## Common Properties

- [Website](https://signal.org/)
- [Documentation](https://signal.org/docs/)
- [Blog](https://signal.org/blog/)
- [Support](https://support.signal.org/)
- [TermsOfService](https://signal.org/legal/)
- [PrivacyPolicy](https://signal.org/legal/#privacy-policy)
- [GitHub](https://github.com/signalapp)

## Capabilities

### Workflow Capabilities

- [Secure Messaging](capabilities/secure-messaging.yaml) — Unified workflow for Signal server operations: account management, device provisioning, pre-key distribution, and encrypted message delivery.

### Shared API Definitions

- [Signal Server](capabilities/shared/signal-server.yaml) — Per-API shared definition for the Signal Server REST API

## Maintainers

**FN:** Kin Lane

**Email:** kin@apievangelist.com
