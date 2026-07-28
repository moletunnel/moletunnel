# Mole — Privacy-First Xray VPN & Proxy Client for Android

**Mole** is a free, privacy-first **VPN and proxy client** powered by **Xray-core**. It is built with **Flutter** for Android (with Windows and Linux desktop builds in system-proxy mode), and focuses on **anti-censorship**, **internet freedom**, and **secure browsing** — with no accounts, no tracking, and no analytics.

Mole supports the modern proxy protocols used to **bypass internet censorship and DPI (Deep Packet Inspection)**: **VLESS (with REALITY and XTLS Vision), VMess, Trojan, Shadowsocks, and Hysteria2**.

---

## Why Mole?

- 🔒 **Privacy first** — no sign-up, no account, no telemetry. Your servers and settings stay on your device.
- 🚀 **Xray-core engine** — the battle-tested core behind the most effective censorship-circumvention tools.
- 🛡️ **Anti-censorship built in** — REALITY, uTLS fingerprints, TLS ClientHello fragmentation, SNI tricks, and padding to evade DPI and firewalls.
- 📱 **Native Android VPN** — full-device tunnel via Android VpnService, with always-on VPN support.
- 🌍 **Multilingual** — English, Persian (Farsi, RTL), Armenian, Russian, and Chinese.

---

## Supported Protocols

| Protocol | Highlights |
|---|---|
| **VLESS** | REALITY, XTLS Vision flow (`xtls-rprx-vision`), TLS, uTLS fingerprints |
| **VMess** | Standard URI links, legacy base64 links, and raw JSON configs |
| **Trojan** | TLS-based, firewall-resistant |
| **Shadowsocks** | AEAD ciphers incl. Shadowsocks-2022 (`2022-blake3-*`), SIP002 links |
| **Hysteria2** | QUIC-based, fast on lossy networks, `hy2://` links |

### Transports & Security

- **TCP (raw)**, **WebSocket (ws)**, **gRPC**, and **XHTTP (SplitHTTP)** transports
- **TLS**, **REALITY** (public key, short ID, SpiderX), and plain modes
- **uTLS fingerprint** spoofing (Chrome and others), custom SNI, ALPN
- **Mux multiplexing** and traffic **sniffing** (HTTP / TLS / QUIC)

---

## Key Features

### Server Management
- Import servers by **share link**, **QR code scan**, **clipboard**, or **raw Xray JSON**
- **Subscription support** with auto-detection: plain link lists, **base64**, **Clash YAML**, **SIP008**, and full JSON subscriptions
- Subscription **quota and expiry tracking** (upload / download / total / expiration)
- Auto-update subscriptions on launch, custom User-Agent per subscription
- Search, sort (name / latency / protocol), filter, pin favorites, bulk delete
- **Share servers** back out as links or QR codes

### Speed & Latency Testing
- **HTTP ping** (true end-to-end test through the tunnel), **TCP connect**, and **ICMP** ping
- **Test All** servers at once and **auto-pick the best server**

### Smart Routing & Split Tunneling
- **Per-app VPN (split tunneling)** — blacklist or whitelist any installed app
- Custom **domain rules**: Proxy / Direct / Block per domain
- Region presets for **Iran, China, and Russia** routing rules
- **Bypass LAN** and **block IPv6 leaks**
- GeoIP / GeoSite rule files with one-tap in-app updates

### Secure DNS
- **DNS-over-HTTPS (DoH)** and **DNS-over-TLS (DoT)**
- **FakeIP** mode for faster, leak-resistant resolution
- Built-in presets: **Cloudflare, AdGuard, AdGuard Family, Quad9, NextDNS, OpenDNS** and custom servers
- DNS filtering: **block ads, malware, trackers, and adult content**

### Anti-Censorship / DPI Evasion
- Evasion profiles: **Light / Moderate / Aggressive**
- **TLS ClientHello fragmentation** with tunable packet size and delay
- Packet **padding** and **mixed-case SNI**

### Everyday Usability
- One-tap **connect dial** with live connection timer and **real-time upload/download speed**
- Live **log viewer** with filtering and export
- **Light / Dark / System themes**
- VPN engine runs in a **separate Android process** for stability; `allowBackup` disabled for privacy

---

## Platforms

| Platform | Status |
|---|---|
| **Android** | ✅ Full VPN (TUN) support — primary platform |
| **Windows** | ✅ Proxy mode (local SOCKS/HTTP + system proxy) |
| **Linux** | ✅ Proxy mode (GNOME system proxy) |
| **iOS / macOS** | 🚧 In development (Network Extension groundwork in place) |

---

## Who Is Mole For?

Mole is for anyone who needs **uncensored, private internet access**:

- Users behind **national firewalls** (Iran, China, Russia and beyond) looking for a **free VPN alternative** that actually works against DPI
- Privacy-conscious users who want a **no-account, no-log client** they fully control
- Self-hosters running their own **VLESS / REALITY / Hysteria2 / Shadowsocks servers**
- Anyone migrating from clients like **v2rayNG, Happ, Nekobox, or Hiddify** who wants a clean, modern Flutter UI

---

## Frequently Asked Questions

**Is Mole free?**
Yes. Mole is a free client. You connect to your own servers or servers from any subscription provider you trust.

**Does Mole collect my data?**
No. There is no account system, no analytics, and no telemetry. Configurations are stored locally (with encrypted storage for sensitive data).

**Does Mole work against DPI censorship?**
Yes — that is its core purpose. REALITY, uTLS fingerprints, XHTTP, Hysteria2, and TLS fragmentation are all designed to defeat modern DPI systems.

**Which VPN protocols does Mole support?**
VLESS (REALITY / XTLS Vision), VMess, Trojan, Shadowsocks (including Shadowsocks-2022), and Hysteria2.

**Can I choose which apps use the VPN?**
Yes — per-app split tunneling lets you include or exclude any installed Android app.

---

## Keywords

`vpn client` · `xray core` · `xray client android` · `vless client` · `reality protocol` · `xtls vision` · `vmess` · `trojan protocol` · `shadowsocks client` · `hysteria2 client` · `anti-censorship` · `bypass gfw` · `bypass internet censorship` · `dpi bypass` · `free vpn android` · `v2ray client` · `proxy client flutter` · `split tunneling android` · `dns over https` · `privacy vpn no logs`

---

*Mole is an independent open client for the Xray-core ecosystem. It does not provide servers — you bring your own or use any compatible subscription.*
