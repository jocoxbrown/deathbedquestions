# Death Bed Questions website

This is the Jekyll source for deathbedquestions.com.

## Publish a writing

Writings live in the `_posts` folder, one file per piece. Each one appears automatically as a card on the Writings page and gets its own page at `/writings/your-title/`.

1. Copy `_posts/POST-TEMPLATE.md` and name the copy `YYYY-MM-DD-your-title.md` (the date sets the order, newest first; it is not shown on the site).
2. Fill in the details at the top:
   - `title`: the title of the piece.
   - `category`: `Letter` or `Reflection` (any new word creates a new filter button).
   - `description`: one sentence shown on the card.
   - `flower`: optional, the pressed flower shown on its card, e.g. `/assets/images/home/dried-lace.webp`. Leave empty and one is picked automatically.
     Available: `dried-lace`, `dried-delphinium-bloom`, `dried-yellow-stem`, `dried-hydrangea-branch`, `dried-cream-branch`, `dried-delphinium-stem`, `dried-hydrangea`, `dried-delphinium-flower`.
   - `featured: true` puts it in the large "Start here" spot (only one at a time).
   - `signoff`: optional, e.g. `"With love, Jo"`.
3. Write the piece below the second `---` line, with an empty line between paragraphs.
4. Delete the line `published: false` when it is ready to go live.

## Shared memories

The "Add your voice" section at the bottom of the Writings page lets visitors answer the question of the month or share a memory. Nothing appears on the site automatically: every submission is read first, then added by hand.

**Where submissions go.** By default the Share button opens the visitor's email app with their words addressed to `memories_email` in `_config.yml`. To receive them without an email app, create a free form at a service such as [Formspree](https://formspree.io), then paste its endpoint into `memories_form` in `_config.yml`, e.g. `memories_form: "https://formspree.io/f/abcdwxyz"`.

**Publishing one.** Open `_data/memories.yml` and add it under `entries` (newest first):

```yaml
entries:
  - text: "The sound of my dad's key in the door at night."
    signed: "A daughter in Cork"   # optional, shows "Anonymous" if left out
    kind: answer                    # answer (to the question) or memory
```

Only publish submissions where the sharing box was ticked, and remove any names or details that could identify someone.

**Changing the question.** Edit `question` and `card` at the top of `_data/memories.yml`. Card images are in `assets/images/home` (e.g. `card-most-alive.webp`).
