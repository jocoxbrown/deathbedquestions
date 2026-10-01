# Death Bed Questions website

This is the Jekyll source for deathbedquestions.com.

## Publish a writing

Writings live in the `_posts` folder, one file per piece. Each one appears automatically as a card on the Writings page and gets its own page at `/writings/your-title/`.

1. Copy `_posts/POST-TEMPLATE.md` and name the copy `YYYY-MM-DD-your-title.md` (the date sets the order, newest first; it is not shown on the site).
2. Fill in the details at the top:
   - `title`: the title of the piece.
   - `category`: `Letter` or `Reflection` (any new word creates a new filter button).
   - `description`: one sentence shown on the card.
   - `image`: optional, e.g. `/assets/images/home/my-photo.webp`. Leave empty for a soft quote-mark card.
   - `featured: true` puts it in the large "Start here" spot (only one at a time).
   - `signoff`: optional, e.g. `"With love, Jo"`.
3. Write the piece below the second `---` line, with an empty line between paragraphs.
4. Delete the line `published: false` when it is ready to go live.
