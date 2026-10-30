# Reading Catalog

A living shelf list and daily reading log for Mitch and his son.

**Books on the shelf:** [catalog.md](catalog.md)  
**What we read each night:** [read.md](read.md)  
**Covers:** [covers/](covers/) (50 local JPEGs)

Repo: [ibmmac/reading-catalog](https://github.com/ibmmac/reading-catalog)

## How to update it every day

1. Open [read.md](read.md) and add a new date heading at the **top** of the log.
2. List each book read, who read it, and any favorite or notes.
3. If it is a new book, add a card in [catalog.md](catalog.md) and drop a JPEG in `covers/`.
4. Commit and push.

Or just send a photo of the book and ask to add it.

## Files

| File | What it is |
| --- | --- |
| [catalog.md](catalog.md) | Books on the shelf, with covers (numbered 1-50) |
| [read.md](read.md) | Daily reading log, newest night first |
| [covers/](covers/) | Local JPEG of every cover |
| [covers/README.md](covers/README.md) | Full filename-to-title map |
| [.github/workflows/store-covers.yml](.github/workflows/store-covers.yml) | Manual workflow to download missing covers from the web |
| README.md | This page |

## Instructions for Grok Bot

When asked to update the catalog:

1. **Read both** `catalog.md` and `read.md` before editing. The next book number is one past the highest in `catalog.md`.
2. **Add books to `catalog.md`** as numbered cards (### N. Title) with author, ISBN, about, and a cover image line: `![Cover of Title](covers/short-name.jpg)`.
3. **Add the night to `read.md`** under a `### YYYY-MM-DD — weekday` heading at the top of the log, with Book / Who read / Notes lines.
4. **Store covers as local JPEGs** in `covers/`. Prefer a cropped photo of the actual copy. Web URLs are fallbacks only — Open Library often returns 1x1 placeholder GIFs, so always check file size (>2 KB) before committing.
5. **Do not renumber** existing cards. Append only.
6. **Keep `covers/README.md`** in sync: every file in `covers/` must appear in its table.
7. One commit per update session is fine. Message style: `Add <title> (#N) and log <date>`.

## Conventions

- Reader: Mitch (Dad), also Amy.
- Started: August 27, 2026.
- McCloskey treasury is one shelf card; track which stories are read inside it.
- Returned library loans stay in `catalog.md` under "Returned library loans" with status noted.
- Indian Subcontinent editions get a note on the card.
- School-library stamps (e.g. *Cleary*, Building #19) get noted but the book is treated as a home copy unless Mitch says otherwise.
