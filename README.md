# Node-Flow: A Minimalist BitTorrent Client in Go

![Go Version](https://img.shields.io/badge/Go-1.20+-00ADD8?style=flat&logo=go)
![License](https://img.shields.io/badge/License-GPL_3.0-blue.svg)

**Node-Flow** is a lightweight, educational implementation of the BitTorrent protocol written in Go. It is designed to demonstrate how peer-to-peer (P2P) file sharing works under the hood, stripping away the complexities of modern clients to focus on the core protocol mechanics.

## 🚀 Features

* **Bencoding Parser:** Decodes `.torrent` files from raw binary data.
* **Tracker Communication:** Connects to HTTP trackers to discover peers.
* **P2P Handshake:** Implements the standard BitTorrent handshake protocol.
* **Parallel Downloads:** Manages concurrency using Go routines to download file pieces from multiple peers simultaneously.
* **Pipelining:** Efficiently queues requests for blocks to maximize throughput.

## ⚠️ Current Limitations

This client is built for educational simplicity and has specific constraints:
* **Single-file torrents only** (Multi-file torrents are not supported).
* **HTTP Trackers only** (UDP trackers and Magnet links are not supported).
* **IPv4 only.**

## 🛠️ Installation & Setup

### Prerequisites
* [Go (Golang)](https://go.dev/dl/) installed on your machine.

### Clone the Repository
```bash
git clone [https://github.com/ARZU-V/Node-Flow.git](https://github.com/ARZU-V/Node-Flow.git)
cd Node-Flow