# SuiteTDD

**AI-Powered NetSuite Technical Design Documents — generated locally on your Mac.**

SuiteTDD is a native macOS app that helps NetSuite consultants and developers produce professional Technical Design Documents (TDDs) in seconds. It runs entirely offline using Apple Silicon's MLX framework — your client data never leaves your Mac.

> Made by Mounir, in Toronto

---

## What's New in v4.0

- **Supabase-backed free trials** — enter your email to start a 7-day trial; one trial per email and per machine, enforced server-side
- **Hard paywall at expiry** — the app fully locks when the trial ends, prompting you to purchase a license
- **`.suitetddlicense` file activation** — double-click a license file to activate instantly, no copy-pasting keys
- **Post-purchase license page** — after Stripe checkout you're redirected to your license key with a one-click download of the license file
- **PDF/Word document import** — import an existing TDD from PDF or Word and SuiteTDD rebuilds it as an editable, structured document using AI
- **AI chat refinement panel** — have a conversation with the AI to iteratively refine generated sections
- **Chat apply validation** — AI-suggested edits are validated before being applied to prevent corruption
- **4-hour online re-check** — trial and license status are re-verified periodically while the app is running

---

## Features

### Local AI Generation
- Runs 100% offline using Apple's MLX framework on Apple Silicon
- Multiple model support — download and switch between models from Settings

### Structured Document Authoring
- Capture everything a TDD needs: client, SOW #, project name, title, solution type, script types, included records, included fields, integration points, testing criteria, risks & assumptions
- NetSuite record autocomplete — 85+ standard records with categorized suggestions
- Expanded field types — all standard NetSuite field types
- Live status workflow: **Draft > Client Review > Client Approved > Cancelled**

### Multi-Document Workspace
- Command Center dashboard with document metrics, recent work, and client browser
- Sidebar with color-coded status badges
- Search across all document fields from the toolbar
- Filter by Client, Status, or Script Type with per-status counts
- Group by Client for a folder-style view
- Duplicate and export documents from the right-click context menu

### Smart Prompt Engineering
- Customize TDD Sections — choose which sections appear, reorder them, write per-section AI instructions and sample text
- Per-section placeholders: `{company}`, `{author}`, `{authorRole}`, `{client}`, `{project}`, `{title}`, `{sow}`, `{date}`
- Global tone/style and additional instructions applied to every generation

### Style System
- Multi-profile styles — create, duplicate, rename, delete, and set a default
- PDF style import — drop a branded PDF and SuiteTDD extracts fonts, sizes, colors, margins, heading styles, and logos automatically

### Live Markdown Preview & Editor
- Side-by-side mode — edit markdown on the left, see the rendered preview on the right
- Inline markdown editor with dark-mode-aware syntax highlighting
- Properly formatted tables, code blocks, and headings

### Import & Export
- One-click export to `.docx`
- Import from PDF or Word — AI extracts and restructures content into editable TDD fields
- Import/export `.suitetdd` files to share between Macs or team members
- Export filename template with `{title}`, `{client}`, `{project}`, `{sow}`, `{date}` placeholders
- Auto status bump — exporting a Draft transitions it to Client Review (configurable)

### Licensing & Free Trial
- 7-day free trial — enter your email to start, no credit card required
- Trial enforced server-side: one per email and one per machine
- Purchase a lifetime license via Stripe — key delivered by email instantly
- Activate by entering a key, or double-click a `.suitetddlicense` file
- Activate on up to 2 machines per license
- Retrieve your license anytime at [suitetdd.com/license-lookup](https://suitetdd.com/license-lookup)

### Keyboard Shortcuts
- **Cmd+N** — New TDD
- **Cmd+Shift+G** — Generate
- **Cmd+P** — Toggle Preview
- **Cmd+E** — Export to Word
- **Cmd+Shift+I** — Import Document
- **Cmd+Option+I** — Import from PDF/Word

### Onboarding & Auto-Update
- First-launch tutorial walks through profile setup, model download, and feature overview
- Built-in auto-update from GitHub Releases — checks daily
- Tutorial re-playable anytime from Settings

---

## Requirements

- macOS 14.0 (Sonoma) or later
- Apple Silicon Mac (M1, M2, M3, M4, or newer)
- ~5 GB of free disk space per AI model

---

## Installation

1. Download the latest DMG from the [Releases page](../../releases/latest)
2. Open the DMG and drag **SuiteTDD.app** into your Applications folder
3. Launch SuiteTDD — signed and notarized by Apple
4. Follow the in-app tutorial to set up your profile and download an AI model

---

## Screenshots

| Command Center | Document Editor |
| --- | --- |
| ![Dashboard](docs/screenshots/dashboard.png) | ![Editor](docs/screenshots/editor.png) |

| Generated Preview | AI Chat Refinement |
| --- | --- |
| ![Preview](docs/screenshots/preview.png) | ![Chat](docs/screenshots/chat.png) |

| PDF/Word Import | License Activation |
| --- | --- |
| ![Import](docs/screenshots/import.png) | ![License](docs/screenshots/license.png) |

---

## Links

- [Purchase a License](https://buy.stripe.com/4gMdR98IUaRNgx6fbgbwk01)
- [Retrieve Your License Key](https://suitetdd.com/license-lookup)
- [Report an Issue](https://github.com/mounirelchoueiri/SuiteTDD-MacOS/issues/new)
- [Release Notes](../../releases)

---

## License

Copyright 2026 Mounir El Choueiri. All rights reserved.

SuiteTDD requires a license for continued use after the 7-day free trial.
