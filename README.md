# EPOCH

**A manual, append-only Unix timestamp log.**

Single HTML file. No server. No dependencies. No accounts.  
Download, open in browser, start logging.

---

## What it is

EPOCH records events as atomic, irreversible entries:

```
1774480360 | default  | woke up
1774480421 | anchor   | session start
1774480890 | flagged  | distraction
```

Each entry is a Unix timestamp, a state, and a short text payload.  
No edits. No deletes. A galvanized register.

---

## Install

```
1. Download index.html
2. Open in any modern browser
3. Done
```

No build step. No npm. No cloud.  
Your data lives in your browser's `localStorage` — it never leaves your machine.

## Download

[**→ Download EPOCH**](https://raw.githubusercontent.com/morphysm/epoch/main/index.html)

*Right-click the link → Save Link (index.html) As → open in browser.*

Or visit the [live demo](https://morphysm.github.io/epoch) to try it first.

---

## Usage

### Logging
Type in the input field at the bottom. Press **Enter** to commit.  
The current Unix timestamp is captured at the moment of submission.

### Entry States
Each entry can be marked after the fact:

| Action | Result |
|---|---|
| Swipe right / right-click | Anchor — green timestamp |
| Swipe left / Ctrl+click | Flagged — red timestamp |
| Swipe again | Revert to default |

States are mutually exclusive. The entry content is never altered.

### ISO Preview
Hold an entry (500ms on desktop, long-press on mobile) to see a temporary  
ISO 8601 human-readable date. Disappears on release. Not stored.

### Keyboard Shortcuts

| Shortcut | Action |
|---|---|
| `Ctrl+E` | Export log (or selection if any entries are green) |
| `Ctrl+Shift+E` | Export with AT+/− notation |
| `Ctrl+H` | Toggle README / help |
| `/calc` + Enter | Open AT calculator |
| `Escape` | Close any open panel |

### Selective Export
Right-click any entries to mark them green (anchor).  
`Ctrl+E` will export only the green ones.  
With no entries selected, `Ctrl+E` exports the full log.

Export format:
```
timestamp|state|content
1774480360|anchor|session start
1774480890|flagged|distraction
```

---

## AT+/− Time

EPOCH includes an Atomic Time calculator and notation system.

**AT+/N** = N years after July 16, 1945 (Trinity test — first nuclear detonation).  
**AT−/N** = N years before 1945.

```
AT+/81  →  2026
AT+/0   →  1945
AT-/169 →  1776
```

Type `/calc` in the input to open the converter.  
Accepts: Unix integers, `YYYY/MM/DD` dates, `AT+/N/MM/DD` notation.

The AT system is a proposal: that time should be counted from the moment  
the species became technically capable of self-annihilation.  
It serves not as a pessimistic approach; rather, as an orientation.

---

## Ghost Scroll

Hover the right edge of the screen to reveal a minimal scroll strip.  
Drag to jump through the log. Works on touch too.

---

## Philosophy

> *Time is atomic, irreversible, and raw.*

EPOCH does not offer:
- Editing
- Deleting
- Cloud sync
- Categories
- Reminders
- Analytics

It offers one thing: a precise record of when things happened, in the order they happened, that cannot be altered after the fact.

A typo in the log is a fact about the moment it was entered. It stays.

---

## Export Format

Files are saved as `.txt`, one entry per line:

```
timestamp|state|content
```

Chronological order, oldest first. Pipe-delimited. No header.  
Machine-readable and human-readable without any tooling.

## Further Reading

[AT+/− · Time, Trinity, and the Mechanics of EPOCH](AT_calendar_history.md)

---

## License

Do what you want with it.  
If you build something with it, a mention is appreciated but not required.

---

*J.K., Norrland XXVI*
*AT+/81*
