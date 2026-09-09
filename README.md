# Grasp landing page

> Don’t outsource your understanding.

The public site for [Grasp](https://github.com/silverback-ventures/grasp), a code review tool for the agent era.

One static file, `index.html`. No build step, no JavaScript, and no dependencies beyond the Geist fonts loaded from Google Fonts. The page is a single screen: the wordmark, the headline, and one call to action.

The colors and type follow the Grasp design system: black canvas, white foreground, a gray ramp for hierarchy, and one orange accent for the cursor mark and the primary action. The light theme follows the operating system through `prefers-color-scheme`. There is no toggle.

The wordmark cursor is the only thing on the page that animates, and it stops under `prefers-reduced-motion`.

## The headline

The headline is set as two explicit lines. Its size comes from the column width in `cqw` units, so the longer line sits flush to the measure at every viewport rather than stopping short of it. That ratio depends on the tracking: change `letter-spacing` on `.hero h1` and the line will no longer fill the column, so re-derive the `cqw` coefficient if you touch it.

## Run it

Open `index.html` in a browser, or serve the directory:

```bash
python3 -m http.server 8000
```

## Deploy

Any static host works. Point it at the repository root. `.nojekyll` is there for GitHub Pages.
