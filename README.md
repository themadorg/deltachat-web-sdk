# Delta Chat Web SDK — Hierarchical Documentation

The Delta Chat Web SDK is a high-level library for building Delta Chat-compatible messengers in web environments. It is built on top of the Delta Chat Relay protocol (JSON-RPC over WebSocket) and provides a multi-account, PGP-first messaging experience.

---

## 🗺️ Documentation Journey

Choose your entry point based on your needs:

### 🚀 Level 1: SDK Fundamentals
*Target: New developers and evaluators.*
- **[Introduction & Overview](./docs/examples.md#quick-start)**: Why the "Web Mono" SDK exists (zero-backend, PGP-first, email-based).
- **Architecture at a Glance**: How it sits between your UI and Delta Chat Relays.
- **Quick Start**: Installing, registering, and sending your first message.
- **[The Factory Pattern](./docs/examples.md#the-factory-pattern)**: Managing multiple `DeltaChatAccount` instances.

### 📱 Level 2: Core Messaging & Management
*Target: Application developers building messenger features.*
- **[Account Lifecycle](./docs/examples.md#account-lifecycle)**: Registration, connection, and persistence with `IndexedDBStore`.
- **[Unified Messaging (`.send()`)](./docs/examples.md#unified-messaging-send)**: Power of the Unified Payload (Text, Image, Video, Reactions, Edits).
- **[Real-time Event System](./docs/examples.md#receiving-messages--events)**: Listening for incoming messages and connection state changes.
- **[Contacts & Groups](./docs/examples.md#contacts--groups)**: Managing contact lists, groups, and broadcast channels.

### 🔐 Level 3: Security & Advanced Features
*Target: Security-conscious developers and advanced users.*
- **[PGP & Autocrypt](./docs/security.md#pgp--autocrypt)**: Key generation, fingerprint management, and opportunistic encryption.
- **[SecureJoin Handshake](./docs/security.md#securejoin-handshake)**: Deep dive into the QR-code/URI verification protocol.
- **[Multi-Device Synchronization](./docs/security.md#multi-device-synchronization)**: Keeping state consistent across devices.
- **[Media Processing](./docs/security.md#media-processing)**: Base64 handling, MIME parsing, and attachment decryption.

### 🔬 Level 4: Architecture & Protocol Internals
*Target: Core contributors and protocol researchers.*
- **[The WebSocket Protocol](./docs/architecture.md#the-websocket-protocol)**: JSON-RPC message structure and action definitions.
- **[The UID System](./docs/architecture.md#the-uid-system)**: How message tracking and synchronization works.
- **[Internal Modularization](./docs/architecture.md#internal-modularization)**: Understanding `lib/transport.ts`, `lib/crypto.ts`, and `lib/mime.ts`.
- **[Developing Extensions](./docs/architecture.md#developing-extensions)**: Webxdc support and custom storage implementations.

---

## Installation

```bash
npm install deltachat-web-sdk
# or
bun add deltachat-web-sdk
```

---

## License

MIT / GPLv3 (See Delta Chat core licenses for details).
