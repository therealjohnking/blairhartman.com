# blairhartman.com

Source for [blairhartman.com](https://blairhartman.com).

Static HTML + CSS — no build step, no framework, no JavaScript. Deployed to
Cloudflare Workers using Static Assets (see `wrangler.jsonc`, which serves
`./public`). Pushes trigger Cloudflare Workers Builds.

## Structure

```
public/
├── index.html      # the whole page
└── css/
    └── site.css    # the "Workpaper" design system
```

## Updating the "Currently" block

The `Currently` section is deliberately primitive so it stays easy to edit by
hand. In `public/index.html`, find the `<!-- CURRENTLY: update entries and date
together -->` comment and edit the two entries and the `as of …` date in the
same place. The date is plain text (there is no JavaScript) — change it whenever
you change the entries.
