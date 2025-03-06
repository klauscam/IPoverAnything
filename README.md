# IP over Anything

**Tunnel IP traffic over unconventional protocols and mediums—MQTT, WebSockets, HTTP, Databases, SMS, and more.**

## Overview

**IP over Anything** is an innovative and experimental project demonstrating how IP packets can be tunneled through virtually any transport medium or protocol. This flexibility allows for VPN-like connectivity in environments where traditional VPN solutions might be restricted, monitored, or blocked.

This repository includes practical implementations, scripts, and examples of tunneling IP over:
- **MQTT**
- **WebSockets**
- **HTTP (GET/POST)**
- **Databases (MongoDB)**
- **SMS** (planned)

The core mechanism relies on Linux's TUN interface, abstracting layers 1 (Physical), 2 (Data Link), and 3 (Network), thus enabling seamless tunneling through diverse protocols.

## Current Implementations

- **IP over MQTT:** IP packets encapsulated in MQTT messages.
- **IP over WebSockets:** Optimized transport layer using WebSockets.
- **IP over HTTP:** Using standard HTTP requests to tunnel IP data.
- **IP over Databases:** Storing and retrieving IP packets via database records.

## Planned Features

- **IP over SMS:** Adjusting MTU to SMS constraints, minimizing fragmentation.
- **Virtual Layer 1:** Exploring deeper network-layer tunneling to virtualize physical layer connections.
- **Performance optimization:** Rewriting core components in Rust for efficiency and scalability.

## Requirements

- Linux-based system (for TUN/TAP interface support)
- Python
- Dependencies (specified in individual project directories)

## Installation & Usage

1. Clone this repository:
   ```sh
   git clone https://github.com/klauscam/IPoverAnything.git
   ```

2. Navigate to the desired implementation directory, for example:
   ```sh
   cd IPoverAnything/IPoverWebsockets
   ```

3. Follow individual README instructions for setup and execution.

## Contributions

Contributions, improvements, and ideas are warmly welcomed. Feel free to submit pull requests, open issues, or start discussions on GitHub.

## License

This project is licensed under the **GPL-3.0 License**—see the [LICENSE](LICENSE) file for details.

## Disclaimer

This project is intended for educational purposes, research, and authorized security assessments only. Misuse may lead to legal consequences. Use responsibly.

