# SuiteTDD

**AI-Powered NetSuite Technical Design Documents — generated locally on your Mac.**

SuiteTDD is a native macOS app that helps NetSuite consultants and developers produce professional Technical Design Documents (TDDs) in seconds. It runs entirely offline using Apple Silicon's MLX framework — your client data never leaves your Mac.

> Made with ❤️ by Mounir, in Toronto 🇨🇦

---

## Features

### 🧠 Local AI Generation
- Runs 100% offline using Apple's MLX framework on Apple Silicon

### 📄 Structured Document Authoring
- Capture everything a TDD needs: client, SOW #, project name, TDD title, solution type, script types, included records, included fields, integration points, testing criteria, risks & assumptions
- **NetSuite record autocomplete** — 85+ standard records (Sales Order, Invoice, Customer, Vendor, etc.) with categorized suggestions as you type
- **Expanded field types** — all standard NetSuite field types (Date/Time, Percent, Multiple Select, Phone Number, and more)
- Live status workflow per document: **Draft → Client Review → Client Approved → Cancelled**

### 🗂️ Multi-Document Workspace
- Sidebar lists every TDD you've created with color-coded status badges
- **Search** across all document fields from the toolbar — instant filtering as you type
- Filter by **Client** or **Status** with per-status document counts
- Toggle **Group by Client** for a folder-style view
- **Duplicate** documents from the right-click context menu

### ✨ Smart Prompt Engineering
- Customize **TDD Sections** — choose which sections appear, reorder them, write per-section AI instructions and sample text
- Per-section placeholders: `{company}`, `{author}`, `{authorRole}`, `{client}`, `{project}`, `{title}`, `{sow}`, `{date}`
- Global tone/style and "additional instructions" applied to every generation

### 🎨 Style System
- **Multi-profile styles** — create, duplicate, rename, delete, and set a default style profile
- **PDF style import** — drop a branded PDF and SuiteTDD extracts fonts, sizes, colors, margins, heading styles, and logos automatically

### 📝 Live Markdown Preview & Editor
- **Side-by-side mode** — edit markdown on the left, see the rendered preview live on the right
- Inline markdown editor — tweak generated content before exporting
- Web view preview with dark-mode-aware syntax highlighting
- Properly formatted tables, code blocks, and headings

### 📤 Export & Sharing
- One-click export to `.docx` with native macOS save dialog
- **Import/export `.suitetdd` files** — share documents between Macs or team members
- **Export filename template** with `{title}`, `{client}`, `{project}`, `{sow}`, `{date}` placeholders
- **Auto status bump** — exporting a Draft automatically transitions it to Client Review (configurable)

### 🔐 Licensing & Free Trial
- **7-day free trial** with full access — no credit card required
- Purchase a lifetime license via Stripe — key delivered by email instantly
- Activate on up to 2 machines per license

### ⌨️ Keyboard Shortcuts
- **⌘N** — New TDD
- **⌘⇧G** — Generate
- **⌘P** — Toggle Preview
- **⌘E** — Export to Word
- **⌘⇧I** — Import Document

### 🚀 Onboarding & Auto-Update
- First-launch tutorial walks new users through profile setup, model download, feature overview, and trial activation
- Built-in **auto-update** from GitHub Releases — checks daily, downloads DMG, mounts, replaces, and relaunches
- Tutorial re-playable anytime from **Settings → General**

---

## Requirements

- macOS 14.0 (Sonoma) or later
- Apple Silicon Mac (M1, M2, M3, or newer) — MLX requires Apple Silicon
- ~5 GB of free disk space per AI model

---

## Installation

1. Download `SuiteTDD-v3.0.2.dmg` from the [latest release](../../releases/latest)
2. Open the DMG and drag **SuiteTDD.app** into your Applications folder
3. Launch SuiteTDD — it's signed and notarized by Apple, so it opens without any security warnings
4. Follow the in-app tutorial to set up your profile, download an AI model, and start your free trial

---

## Screenshots

<!-- Drop screenshots into docs/screenshots/ and they'll render below -->

| Document Editor | Generated Output |
| --- | --- |
| ![Document Editor](docs/screenshots/editor.png) | ![Preview](docs/screenshots/preview.png) |

| Sidebar with Filters | Settings & TDD Sections |
| --- | --- |
| ![Sidebar](docs/screenshots/sidebar.png) | ![Settings](docs/screenshots/settings.png) |

| AI Models Manager | First-Launch Tutorial |
| --- | --- |
| ![Models](docs/screenshots/models.png) | ![Tutorial](docs/screenshots/tutorial.png) |

---

## Roadmap

- [ ] Template library for common NetSuite customization patterns
- [ ] Email license keys automatically via Resend after Stripe purchase
- [ ] Anything else you can think of and want to request!

---

## License

Copyright © 2026 Mounir El Choueiri. All rights reserved.

SuiteTDD requires a license for continued use after the 7-day free trial. Purchase a license at the in-app "Buy Now" link or from [our website](https://buy.stripe.com/4gMdR98IUaRNgx6fbgbwk01).
