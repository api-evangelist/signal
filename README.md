# Signal (signal)
Signal is a privacy-focused messaging platform that provides end-to-end encrypted communication through open-source applications on mobile and desktop. Their developer ecosystem centers around the open-source Signal Protocol, client SDKs, and server infrastructure, enabling developers to study, audit, and integrate secure messaging capabilities.

**URL:** [Visit APIs.json URL](https://raw.githubusercontent.com/api-evangelist/signal/refs/heads/main/apis.yml)

## Scope

- **Type:** Contract
- **Position:** Consuming
- **Access:** 3rd-Party

## Tags:

 - Encryption, Messaging, Security, Cryptography, Open Source, Privacy

## Timestamps

- **Created:** 2026-03-20
- **Modified:** 2026-03-20

## APIs

### Signal Protocol Specifications
The Signal Protocol Specifications define the core cryptographic protocols that underpin Signal's end-to-end encrypted messaging. These include the X3DH (Extended Triple Diffie-Hellman) key agreement protocol for establishing shared secrets between parties, the Double Ratchet Algorithm for deriving new encryption keys per message, the PQXDH (Post-Quantum Extended Diffie-Hellman) protocol for quantum-resistant key agreement, and XEdDSA for EdDSA-compatible signature schemes. These specifications are published independently so they can be adopted by other projects beyond Signal itself.

**Human URL:** [https://signal.org/docs/](https://signal.org/docs/)


#### Tags:

 - Encryption, Messaging, Cryptography, Security, Protocols

#### Properties

- [Documentation](https://signal.org/docs/)

### Signal libsignal SDK
The libsignal SDK provides platform-agnostic APIs used by the official Signal clients and server. It implements the Signal Protocol including the Double Ratchet algorithm, as well as other cryptographic primitives such as AES-GCM encryption and zero-knowledge group functionality. The core implementations are written in Rust, with bindings exposed as Java, Swift, and TypeScript libraries. Developers building applications that need Signal-compatible end-to-end encryption can integrate libsignal to handle key exchange, message encryption, and decryption.

**Human URL:** [https://github.com/signalapp/libsignal](https://github.com/signalapp/libsignal)


#### Tags:

 - SDK, Encryption, Cryptography, Java, Swift, TypeScript, Rust

#### Properties

- [Documentation](https://github.com/signalapp/libsignal)

### Signal Server
Signal-Server is the open-source server backend that supports the Signal Private Messenger applications on Android, Desktop, and iOS. Built as a Dropwizard application, it provides REST controllers for account management, message delivery, key distribution, and device provisioning, along with gRPC services and WebSocket endpoints for real-time communication. The server handles user registration, encrypted message routing, push notification delivery, and pre-key bundle management. While Signal does not offer an official public REST API for third-party use, the server source code is available for inspection and self-hosting.

**Human URL:** [https://github.com/signalapp/Signal-Server](https://github.com/signalapp/Signal-Server)


#### Tags:

 - Messaging, Server, Backend, Encryption, Open Source

#### Properties

- [Documentation](https://github.com/signalapp/Signal-Server)
- [OpenAPI](openapi/signal-server-openapi.yml)
- [AsyncAPI](asyncapi/signal-server-asyncapi.yml)

### Signal Android SDK
Signal-Android is the open-source Android client for the Signal encrypted messaging platform. It provides the full messaging experience including end-to-end encrypted text messages, voice calls, video calls, group chats, and media sharing. The application integrates the libsignal protocol library for cryptographic operations and communicates with the Signal Server for message routing and delivery. The source code is publicly available, allowing developers to study the implementation of secure messaging on the Android platform.

**Human URL:** [https://github.com/signalapp/Signal-Android](https://github.com/signalapp/Signal-Android)


#### Tags:

 - Android, Mobile, Messaging, Encryption, Open Source

#### Properties

- [Documentation](https://github.com/signalapp/Signal-Android)

### Signal iOS SDK
Signal-iOS is the open-source iOS client for the Signal encrypted messaging platform. It delivers end-to-end encrypted messaging, voice calls, video calls, and group communications on iPhone and iPad devices. The application uses the libsignal protocol library for all cryptographic operations and connects to the Signal Server infrastructure for message delivery and synchronization. The codebase is publicly available on GitHub, enabling developers to review the secure messaging implementation for Apple platforms.

**Human URL:** [https://github.com/signalapp/Signal-iOS](https://github.com/signalapp/Signal-iOS)


#### Tags:

 - iOS, Mobile, Messaging, Encryption, Open Source

#### Properties

- [Documentation](https://github.com/signalapp/Signal-iOS)

### Signal Desktop SDK
Signal-Desktop is the open-source desktop client for the Signal encrypted messaging platform, built with Electron and TypeScript. It provides end-to-end encrypted messaging, voice calls, video calls, and group communications on Windows, macOS, and Linux. The desktop client links to an existing Signal mobile account and synchronizes messages across devices. It integrates the libsignal TypeScript bindings for cryptographic operations and maintains the same security guarantees as the mobile applications.

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

## Maintainers

**FN:** API Evangelist

**Email:** info@apievangelist.com
