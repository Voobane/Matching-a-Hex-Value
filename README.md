# 🎨 Matching a Hex Value — Regex Tutorial

A GitHub Gist-style tutorial that breaks down the regular expression used to validate hexadecimal color codes: `/^#?([a-f0-9]{6}|[a-f0-9]{3})$/`. Written as a beginner-friendly deep dive into regex components using a real-world example.

---

## 📖 Overview

Regex can look like gibberish at first glance. This tutorial takes one practical pattern — hex color validation — and explains every piece of it so that a developer new to regex walks away understanding not just *what* it matches, but *why*.

The regex covered: `/^#?([a-f0-9]{6}|[a-f0-9]{3})$/`

---

## ✨ What the Tutorial Covers

- ⚓ **Anchors** (`^`, `$`) — ensuring the entire string matches, not just part of it
- 🔢 **Quantifiers** (`{3}`, `{6}`) — setting exact character counts
- 🔀 **Grouping and OR** (`()`, `|`) — matching either a 3-digit or 6-digit hex code
- 🧩 **Bracket Expressions** (`[a-f0-9]`) — defining the valid set of hex characters
- `#?` — making the leading `#` optional

---

## 🛠️ Tech Stack

| | |
|---|---|
| Format | Markdown (GitHub Gist) |
| Subject | Regular Expressions (JavaScript) |

---

## 💡 What I Learned

- How **regex anchors** (`^` and `$`) enforce full-string matching
- How **bracket expressions** define character classes
- How the **alternation operator** (`|`) lets a pattern match multiple formats
- How to read and explain a regex pattern component by component

---

## 👤 Author

**Matt (Voobane)**
- GitHub: [@Voobane](https://github.com/Voobane)
