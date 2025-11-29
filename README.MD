# ChatUncontrol

<div align="center">
  <img src="icon.png" alt="ChatUncontrol Logo" width="128" height="128">

  **Privacy-focused messaging platform with end-to-end encryption**

  [![Version](https://img.shields.io/badge/version-0.6.0-blue.svg)](https://github.com/plumsydev/ChatUncontrol/releases)
  [![Codename](https://img.shields.io/badge/codename-Pulse-purple.svg)](https://github.com/plumsydev/ChatUncontrol)

  [Roadmap](https://chatuncontrol.app/roadmap) | [Download Desktop](https://github.com/plumsydev/ChatUncontrol/releases)
</div>

---

## Overview

ChatUncontrol is a secure, privacy-first messaging application that puts you in control of your communications. Built with end-to-end encryption using the **Fuck-Feds Custom Protocol (FFCP)**, ChatUncontrol ensures that your messages, calls, and files remain private and secure.

### Key Features

- **End-to-End Encryption** - All messages, calls, and files are encrypted using state-of-the-art cryptographic protocols
- **No Phone Number Required** - Sign up with just a username and password
- **Disappearing Messages** - Set messages to self-destruct after 1 minute to 7 days
- **Voice & Video Calls** - Encrypted real-time communication
- **Group Chats** - Encrypted group conversations with up to 100 members
- **Message Replies** - Quote and respond to specific messages
- **File Sharing** - Share images, videos, documents with automatic encryption
- **Cross-Platform** - Web, Windows Desktop (macOS & Linux coming soon)
- **Dark & Light Themes** - Customizable appearance
- **Offline Support** - PWA with service worker for offline capabilities

---

### Technology Stack

| Component | Technologies |
|-----------|-------------|
| **Backend** | Go 1.22+, Gin, PostgreSQL, WebSocket, JWT |
| **Frontend** | React 18, TypeScript, Vite, Tailwind CSS, Zustand |
| **Desktop** | Electron 33, React, TypeScript, electron-builder |
| **Encryption** | XChaCha20-Poly1305, X25519, Argon2id |

---

## Security

### Encryption Protocol (FFCP v0.7.1)

ChatUncontrol uses the **Fuck-Feds Custom Protocol** for end-to-end encryption:

- **Key Exchange**: X25519 Elliptic Curve Diffie-Hellman
- **Message Encryption**: XChaCha20-Poly1305 (AEAD)
- **Key Derivation**: Argon2id for password hashing
- **Perfect Forward Secrecy**: Double Ratchet algorithm
- **File Encryption**: Automatic client-side encryption before upload

### Privacy Features

- No phone number required for registration
- No message metadata stored on servers
- Messages stored encrypted (server cannot read content)
- Disappearing messages with configurable timers
- Local-first architecture with minimal data collection

---

## Features in Detail

### Messaging

- **Text Messages** with emoji support (shortcode autocomplete `:smile:`)
- **Message Replies** - Quote and respond to specific messages
- **Message Editing** - Edit your sent messages
- **Message Deletion** - Delete messages for everyone
- **Reactions** - React to messages with emojis
- **Link Previews** - Automatic preview for shared URLs
- **Typing Indicators** - See when others are typing

### Voice & Video Calls

- **1-on-1 Calls** - Private audio and video calls
- **Group Voice Calls** - Up to 8 participants
- **Encrypted** - All call media is end-to-end encrypted
- **Adaptive Bitrate** - Quality adjusts based on network conditions

### Groups

- **Encrypted Group Chats** - Up to 100 members
- **Admin Controls** - Add/remove members, change settings
- **Group Info** - Custom name and description

### File Sharing

- **Images** - Direct preview in chat
- **Videos** - Built-in video player
- **Voice Messages** - Record and send audio clips
- **Documents** - Share PDF, DOC, and other files
- **Automatic Encryption** - Files encrypted before upload

### Desktop App Features

- **System Tray** - Run in background for notifications
- **Auto-Updates** - Automatic updates via GitHub releases
- **Native Notifications** - OS-level notifications
- **Splash Screen** - Animated loading with update progress

---

## Roadmap

See the full [Roadmap](https://chatuncontrol.app/roadmap) for detailed changes.

---

## Acknowledgments

- [Vite](https://vitejs.dev/) - Next Generation Frontend Tooling
- [Tailwind CSS](https://tailwindcss.com/) - Utility-first CSS framework
- [Zustand](https://github.com/pmndrs/zustand) - Small, fast state management
- [Gin](https://gin-gonic.com/) - HTTP web framework for Go
- [Electron](https://www.electronjs.org/) - Cross-platform desktop apps
- [libsodium](https://doc.libsodium.org/) - Modern cryptography library

---

<div align="center">
  <b>ChatUncontrol</b> - Secure • Private • Free
  <br>
  <sub>Privacy is not a crime.</sub>
</div>
