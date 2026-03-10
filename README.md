# robots.md — The AI Agent Discovery Standard

A proposal for a new open standard that helps AI agents discover and understand your business.

## 🌐 Live Demo

View the specification at: **[agenti.nz/robots-md-standard.html](https://agenti.nz/robots-md-standard.html)**

## 📋 What is robots.md?

`robots.md` is a Markdown file placed at the root of a website that provides AI agents with structured, human-readable information about a business and its available digital interfaces.

Think of it as the modern evolution of `robots.txt` — designed specifically for the age of AI agents.

## 🔍 The Problem

The web was built for humans and search engines. `robots.txt` (1994) tells crawlers where they can and can't go. But it was never designed for AI agents that:

- Book appointments on behalf of humans
- Compare services programmatically  
- Make purchases automatically
- Integrate systems autonomously

These agents don't need HTML layouts or meta descriptions. They need **structured, machine-readable content** that describes what a business does, what APIs are available, and how to interact programmatically.

## ✨ Key Features

- **Human-readable first** — Written in Markdown, editable in any text editor
- **Progressive complexity** — Start with 10 lines, add depth as needed
- **Complementary** — Works alongside robots.txt, sitemap.xml, and JSON-LD
- **Privacy by design** — Includes data handling declarations as a required section

## 📄 Files in This Repo

| File | Description |
|------|-------------|
| `robots-md-standard.html` | Full specification page with styling |
| `robots-md-standard-og.jpg` | Social card image for sharing |

## 🚀 Quick Start

Add this to your website's `<head>`:

```html
<link rel="ai-discovery" href="/robots.md" type="text/markdown">
```

Create a `/robots.md` file with:

```markdown
# Your Business Name

## Identity
- Organization: Your Business Name
- Website: https://example.com
- Industry: What you do
- Location: Where you operate
- Contact: hello@example.com
- Updated: 2026-03-10

## Services
A description of what the business offers...

## Data & Privacy
How data is handled, stored, and protected.

## Permissions
- Cache: yes (refresh: 24h)
- Attribution: Required
```

## 🤝 Get Involved

This is an open proposal. We're looking for:

- **Early adopters** — Businesses willing to implement robots.md
- **AI developers** — Build tools that discover and parse robots.md files
- **Contributors** — Help refine the spec and build validators

## 📞 Contact

Proposed by [Agenti NZ](https://agenti.nz) — AI Automation for Kiwi Businesses

- Email: call@agenti.nz
- Website: https://agenti.nz

## 📜 License

This specification is open source. Contributions welcome.
