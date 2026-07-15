# Discord Announcement Editor

A single-page, no-build editor for writing Discord announcements. It gives you toolbar
buttons for every Discord markdown format, plus a live preview that approximates how the
message will render once posted.

Open `index.html` in a browser (or serve it via GitHub Pages) — there's no build step and
no dependencies.

## Features

- Toolbar buttons for all Discord text formatting:
  - Bold, italic, bold-italic, underline, strikethrough, spoiler
  - Inline code and multi-line code blocks
  - Blockquote (`>`) and full-message blockquote (`>>>`)
  - Headers (`#`, `##`, `###`) and subtext (`-#`)
  - Bullet lists and numbered lists
  - Masked links (`[text](url)`) — note: Discord only renders these specially for
    bots/webhooks or inside embeds; in a normal user message they show as plain text.
- Live preview styled like a Discord message (avatar, author, timestamp, formatted body),
  including clickable spoiler tags.
- "Copy raw text" button to grab the plain markdown and paste it straight into Discord's
  message box.

## Discord markdown reference

| Format | Syntax |
| --- | --- |
| Bold | `**text**` |
| Italic | `*text*` or `_text_` |
| Bold italic | `***text***` |
| Underline | `__text__` |
| Strikethrough | `~~text~~` |
| Spoiler | `\|\|text\|\|` |
| Inline code | `` `text` `` |
| Code block | ` ```text``` ` (optionally ` ```lang` for syntax highlighting) |
| Blockquote (line) | `> text` |
| Blockquote (rest of message) | `>>> text` |
| Header 1 / 2 / 3 | `# text`, `## text`, `### text` |
| Subtext | `-# text` |
| Bullet list | `- text` |
| Numbered list | `1. text` |
| Masked link (bots/embeds only) | `[text](url)` |

## Roadmap

This is currently a personal copy/paste tool. A possible next step is a Discord bot that
takes the formatted message from this page and posts it directly into a server channel or
category — not implemented yet.
