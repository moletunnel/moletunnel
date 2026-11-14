<div align="center">

<a href="https://moletunnel.co"><img src="https://moletunnel.co/og.png" alt="Mole — free Xray-core VPN and proxy client" width="760"></a>

# Mole

**A free, privacy-first Xray-core VPN & proxy client for Android, iPhone, iPad, macOS, Windows and Linux.**
Bring your own server or subscription — VLESS · REALITY · VMess · Trojan · Shadowsocks · Hysteria2.

[![Latest release](https://img.shields.io/github/v/release/moletunnel/moletunnel?label=release&color=c74a14)](https://github.com/moletunnel/moletunnel/releases/latest)
[![Downloads](https://img.shields.io/github/downloads/moletunnel/moletunnel/total?color=4f6b3a)](https://github.com/moletunnel/moletunnel/releases)
[![Website](https://img.shields.io/badge/web-moletunnel.co-2a2118)](https://moletunnel.co)
[![Telegram](https://img.shields.io/badge/Telegram-moletunnel-26A5E4?logo=telegram&logoColor=white)](https://t.me/moletunnel)

[Download](#-download) · [Features](#-features) · [Platforms](#-platforms) · [FAQ](#-faq) · [Privacy](https://moletunnel.co/privacy/) · [Docs](https://docs.moletunnel.co)

</div>

---

Mole is a **client**, not a VPN service: it has no servers of its own and no account. You connect it to
your own server or to a subscription from a provider you choose, and your traffic goes straight from
your device to that server — nobody, including us, is in between. It is built on the battle-tested
**Xray-core** engine and is designed for **anti-censorship**: REALITY, uTLS fingerprints, XHTTP, Hysteria2
and traffic masks get through DPI firewalls where ordinary VPNs are blocked.

## 📥 Download

| Platform | Get it | Notes |
|---|---|---|
| **Android** | [**Google Play**](https://play.google.com/store/apps/details?id=com.mole.client) · [APK](https://github.com/moletunnel/moletunnel/releases/latest) | Android 7+ · full-device VPN |
| **iPhone & iPad** | [**App Store**](https://apps.apple.com/app/id6833924268) | iOS 15+ · full-device VPN |
| **macOS** | [`.dmg`](https://github.com/moletunnel/moletunnel/releases/latest) | Apple Silicon |
| **Windows** | [`Setup.exe` / portable `.zip`](https://github.com/moletunnel/moletunnel/releases/latest) | x64 |
| **Linux** | [`.deb` · `.rpm` · `.AppImage` · `.tar.gz`](https://github.com/moletunnel/moletunnel/releases/latest) | x64 |

All desktop installers and the Android APK are attached to each
[**release**](https://github.com/moletunnel/moletunnel/releases/latest), together with a `SHA256SUMS.txt`.

<details>
<summary><b>First launch on macOS / Windows, and verifying a download</b></summary>

- **macOS** — the app is not notarized yet, so Gatekeeper blocks the first launch. Open the `.dmg`,
  drag Mole to **Applications**, then right-click the app → **Open** → **Open** once.
- **Windows** — the installer is unsigned, so SmartScreen warns on first run: **More info** → **Run anyway**.
- **Android APK** — if you previously installed a GitHub APK older than **1.0.29**, uninstall it once
  first: releases are now signed with the same key as Google Play, so the old build can't be upgraded in place.
- **Verify** — download `SHA256SUMS.txt` next to your file, then run
  `sha256sum -c SHA256SUMS.txt --ignore-missing` (macOS: `shasum -a 256 -c SHA256SUMS.txt --ignore-missing`).

</details>

## 🚀 Quick start

1. Install Mole for your platform.
2. Tap **＋** and add your server: paste a **share link** (`vless://`, `vmess://`, `trojan://`, `ss://`,
   `hy2://`), paste a **subscription URL**, scan a **QR code**, or import from the **clipboard**.
3. Pick a server (or let Mole auto-select the fastest one) and press the **connect** button.

## ✨ Features

### Protocols & transports

| Protocol | Highlights |
|---|---|
| **VLESS** | REALITY, XTLS Vision (`xtls-rprx-vision`), TLS, uTLS fingerprints |
| **VMess** | Standard URI links, legacy base64 links, raw JSON configs |
| **Trojan** | TLS-based, firewall-resistant |
| **Shadowsocks** | AEAD ciphers incl. Shadowsocks-2022 (`2022-blake3-*`), SIP002 links |
| **Hysteria2** | QUIC-based, fast on lossy networks, **Salamander** obfuscation, Brutal bandwidth control |

- Transports: **TCP**, **WebSocket**, **gRPC**, **XHTTP** (including stream-one over **HTTP/3**)
- Security: **TLS**, **REALITY** (public key, short ID, SpiderX), uTLS fingerprints, custom SNI and ALPN
- **XMC traffic mask** — disguises the connection as Minecraft traffic where game traffic is allowed
- **Mux** multiplexing and traffic **sniffing** (HTTP / TLS / QUIC)

### Servers & subscriptions
- Import by **share link**, **QR code**, **clipboard** or **raw Xray JSON**
- **Subscriptions** with auto-detection: plain link lists, **base64**, **Clash YAML**, **SIP008** and full
  **Xray JSON** profiles (multi-server balancers with automatic best-server selection)
- Quota and expiry tracking, custom User-Agent per subscription, background refresh (Android)
- Search, sort and filter; **latency tests** (HTTP end-to-end, TCP connect) with one-tap **Test All**

### Routing & DNS
- **Per-app split tunneling** on Android — include or exclude any installed app
- Custom **domain rules** (proxy / direct / block), region presets, **bypass LAN**, **block IPv6 leaks**
- **DNS-over-HTTPS**, **DNS-over-TLS** or plain DNS, **FakeIP**, presets (Cloudflare, AdGuard, Quad9,
  NextDNS, OpenDNS…)
- On-device filtering: **block ads, malware, trackers and adult content**

### Anti-censorship
- Evasion profiles: **Light / Moderate / Aggressive**
- **TLS ClientHello fragmentation**, packet **padding** and **mixed-case SNI**

### Everyday use
- One-tap **connect** with a live timer and real-time upload/download speed
- Live **log viewer**, **light / dark / system** themes
- **5 languages**: English, Persian (RTL), Armenian, Russian, Chinese

## 💻 Platforms

| Platform | Mode |
|---|---|
| **Android** | ✅ Full-device VPN (VpnService), always-on VPN, per-app split tunneling |
| **iPhone & iPad** | ✅ Full-device VPN (Apple Network Extension) |
| **macOS** | ✅ System-proxy mode, plus optional **system-wide VPN mode** (asks for admin / Touch ID) |
| **Windows** | ✅ System-proxy mode, plus optional **system-wide VPN mode** (asks for Administrator) |
| **Linux** | ✅ System-proxy mode, plus optional **system-wide VPN mode** (asks via `pkexec`) |

## 🔒 Privacy

Mole has **no backend, no account, no analytics and no ads**. Your servers, subscriptions and settings are
stored only on your device, and your traffic goes only to the servers you add. Details:
**[moletunnel.co/privacy](https://moletunnel.co/privacy/)**.

## ❓ FAQ

**Is Mole free?**
Yes. Mole is free on every platform. You connect to your own server or to any compatible subscription.

**Is Mole a VPN service? Do you sell servers?**
No. Mole is only the client. You bring a server configuration — your own, or from a provider you trust.

**Does Mole collect my data?**
No. There is no account, no analytics and no telemetry, and we run no servers your data could reach.

**Does it work against DPI censorship?**
That is its core purpose. REALITY, uTLS fingerprints, XHTTP, Hysteria2 with Salamander, the XMC mask and
ClientHello fragmentation are all designed to get through modern DPI.

**Will my provider's subscription work?**
If it gives you VLESS, VMess, Trojan, Shadowsocks or Hysteria2 links — or a Clash, SIP008, base64 or
Xray JSON subscription — yes.

**Where is the source code?**
This repository hosts the **official releases and downloads**. Mole is developed in a separate repository.

## 💬 Support

- **Telegram:** [t.me/moletunnel](https://t.me/moletunnel) — news and support
- **Docs:** [docs.moletunnel.co](https://docs.moletunnel.co)
- **Bugs & feature requests:** [open an issue](https://github.com/moletunnel/moletunnel/issues)
- **Email:** contact@ghyan.dev

---

<div align="center">
<sub>Mole is published by GH Tech, LLC. It is an independent client for the Xray-core ecosystem and does
not provide VPN servers.</sub>
</div>
