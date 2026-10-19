# HBD — handwritten letter

A web page that opens an envelope and writes a message with a pen, one word at a time.
English uses the Satisfy pen font (Vara.js data). Chinese uses Hanzi Writer (correct stroke order). Emoji pop in.

## Change the message

Edit `config.txt`. Settings go above `---`. The message goes below it.

| Setting | Example | Effect |
|---|---|---|
| `to` | `Anna` | Name on the envelope |
| `title` | `A letter for Anna` | Browser tab title |
| `font` | `Satisfy` | English pen font: Satisfy, Parisienne, Pacifico, Shadows Into Light |
| `color` | `#1f2a5a` | Ink color |
| `background` | `paper` | `paper`, or a CSS color for the sheet |
| `speed` | `1.0` | Writing speed multiplier (2.0 = two times faster) |

In the message:
- `{pause 1.5}` stops the pen for 1.5 seconds.
- A line that starts with `>` is right-aligned (use it for the signature).

The link preview text (for chat apps) is at the top of `index.html`.

## Test on your computer

The page must run on a web server (a double-click does not work):

```bash
npx http-server -p 8000 -c-1 .
```

Then open http://localhost:8000.
