# steven95421.github.io

Source of [steven95421.github.io](https://steven95421.github.io/), Steven Yang's personal page.

It is plain hand-written HTML: no build step, no dependencies, no JavaScript.
GitHub Pages serves the root of the `gh-pages` branch as-is, so a push to it is the deploy.

## Files

| File | What it is |
| --- | --- |
| `index.html` | The whole site: markup plus one inline `<style>` block |
| `404.html` | Shown by GitHub Pages for unknown URLs |
| `favicon.svg` | "SY" monogram tab icon |
| `.nojekyll` | Tells GitHub Pages to serve the files without running Jekyll |

## Editing

Open `index.html` in a browser to preview, or run `python3 -m http.server` and visit <http://localhost:8000>.

Every entry under Now, Experience, Projects, Competitions and Education uses the same row markup, so copy a neighbor.
Only `.name` is required; `.role`, `.desc` and `.date` can each be left out.

```html
<div class="row">
  <div class="body">
    <div class="name"><a href="https://example.com/">Name</a></div>
    <div class="role">Role · Team</div>
    <div class="desc">One or two sentences.</div>
  </div>
  <div class="date">2026</div>
</div>
```

- When the Now section changes, bump the `as of …` date in its heading.
- Colors and font stacks are CSS custom properties at the top of the `<style>` block; the dark-mode colors sit right below them.
- `&#8209;` is a non-breaking hyphen and `&#8239;` a narrow non-breaking space. Use them where a line break would strand a fragment, as in `e&#8209;commerce` or `0&#8239;&rarr;&#8239;1`.
