# SuiteTDD

**AI-Powered NetSuite Technical Design Documents — generated locally on your Mac.**

SuiteTDD is a native macOS app that helps NetSuite consultants and developers produce professional Technical Design Documents (TDDs) in minutes. It runs entirely offline using Apple Silicon's MLX framework — your client data never leaves your Mac.

> Made ❤️ by Mounir, in Toronto 🇨🇦

---

## What's New in v4.2

### Performance
- **AI inference off the main thread** — UI stays fully responsive during generation and import
- **Debounced saves** — disk writes batched while typing, with a visual "Saved" indicator
- **Incremental preview updates** — markdown preview no longer flashes or resets scroll on every edit

### Streaming Chat
- **Real-time token streaming** — AI responses appear word-by-word in the chat panel
- **Think-tag filtering** — seamless Qwen3 model compatibility
- **Return to send** — press Return to send, Shift+Return for newline

### UI/UX Polish
- **Required field hints** — red asterisks on required fields, tooltip explains why Generate is disabled
- **Delete confirmation** — documents can no longer be accidentally deleted from the context menu
- **Word count** — word count, character count, and estimated read time in the editor
- **Document count badge** — sidebar footer shows total and filtered document count
- **Clickable outline** — click any heading in the outline panel to scroll the preview to that section
- **Export readiness gate** — export is disabled until all readiness checks pass (title, client, draft, license)

---

## Features

### Local AI Generation
- Runs 100% offline using Apple's MLX framework on Apple Silicon
- Multiple model support — download and switch between models from Settings
- AI processing runs on background threads — UI never blocks during generation

### Structured Document Authoring
- Capture everything a TDD needs: client, SOW #, project name, title, solution type, script types, included records, included fields, integration points, testing criteria, risks & assumptions
- NetSuite record autocomplete — 85+ standard records with categorized suggestions
- Expanded field types — all standard NetSuite field types
- Live status workflow: **Draft > Client Review > Client Approved > Cancelled**
- Required field indicators with clear tooltips

### Multi-Document Workspace
- Command Center dashboard with document metrics, recent work, and client browser
- Sidebar with color-coded status badges and document count
- Search across all document fields from the toolbar
- Filter by Client, Status, or Script Type with per-status counts
- Group by Client for a folder-style view
- Duplicate and export documents from the right-click context menu
- Delete confirmation prevents accidental data loss

### AI Chat Refinement
- Streaming token output — responses appear word-by-word as the AI generates them
- Section-aware Apply — merge AI suggestions into specific document sections
- Insert new sections with placement control
- Single-level undo for applied changes
- Return to send, Shift+Return for multiline input

### Smart Prompt Engineering
- Customize TDD Sections — choose which sections appear, reorder them, write per-section AI instructions and sample text
- Per-section placeholders: `{company}`, `{author}`, `{authorRole}`, `{client}`, `{project}`, `{title}`, `{sow}`, `{date}`
- Global tone/style and additional instructions applied to every generation

### Style System
- Multi-profile styles — create, duplicate, rename, delete, and set a default
- PDF style import — drop a branded PDF and SuiteTDD extracts fonts, sizes, colors, margins, heading styles, and logos automatically

### Live Markdown Preview & Editor
- Side-by-side mode — edit markdown on the left, see the rendered preview on the right
- Incremental preview updates — no flash or scroll reset during editing
- Clickable outline panel — jump to any section in the preview
- Word count, character count, and estimated reading time
- Properly formatted tables, code blocks, and headings

### Import & Export
- One-click export to `.docx` with readiness checklist
- Export gated on all readiness checks (title, client, draft, license)
- Import from PDF or Word — AI extracts and restructures content into editable TDD fields
- Import/export `.suitetdd` files to share between Macs or team members
- Export filename template with `{title}`, `{client}`, `{project}`, `{sow}`, `{date}` placeholders
- Auto status bump — exporting a Draft transitions it to Client Review (configurable)

### Licensing & Free Trial
- 7-day free trial — enter your email to start, no credit card required
- Purchase a lifetime license via Stripe — key delivered instantly & by email
- Retrieve your license anytime at [suitetdd.com/license-lookup](https://suitetdd.com/license-lookup)

### Keyboard Shortcuts
- **Cmd+N** — New TDD
- **Cmd+Shift+G** — Generate
- **Cmd+P** — Toggle Preview
- **Cmd+E** — Export to Word
- **Cmd+Shift+I** — Import Document
- **Cmd+Option+I** — Import from PDF/Word
- **Return** — Send chat message
- **Shift+Return** — Newline in chat

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

## Links

- [Website](https://suitetdd.com)
- [Purchase a License](https://buy.stripe.com/4gMdR98IUaRNgx6fbgbwk01)
- [Retrieve Your License Key](https://suitetdd.com/license-lookup)
- [Report an Issue](https://github.com/mounirelchoueiri/SuiteTDD-MacOS/issues/new)
- [Release Notes](../../releases)

---

## License

Copyright 2026 Mounir El Choueiri. All rights reserved.

SuiteTDD requires a license for continued use after the 7-day free trial.
