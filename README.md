# HyperSend

<p>
    <img alt="License" src="https://img.shields.io/github/license/hypersend-app/hypersend">
</p>

HyperSend is a cross-platform utility designed to move files between devices. It bypasses the cloud, connecting devices directly via LAN or P2P tunnels (QUIC).

## Features

* **Zero-Cloud Storage:** Files move directly from Device A to Device B.
* **Hyper-Fast:** Powered by a Rust core and the QUIC protocol.
* **Cross-Platform:** Windows, Linux, macOS, Android, and iOS.
* **Smart Fallback:** Automatically switches between LAN, Direct P2P, and Relay modes.
* **Resumable:** Transfers handle network drops gracefully.

## Architecture

HyperSend uses a split-process architecture for maximum performance and stability:

* **HyperCore (Rust):** The core library that handles networking, encryption, and file transfers.
* **HyperDaemon (Rust):** Runs as a background service to manage persistent connections.
* **HyperCLI (Rust):** A TUI interface that talks to the Daemon via gRPC for power users and headless environments.
* **HyperClient (Flutter):** A beautiful, cross-platform GUI that talks to the Daemon via gRPC.

## Installation

> We're under development  
> Binaries will be available for all major platforms soon

## License

This project is licensed under the terms of the [AGPL-3.0](https://www.gnu.org/licenses/agpl-3.0.html) license.