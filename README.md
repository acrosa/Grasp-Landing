# Grasp landing page

> Don't outsource your understanding.

The public site for [Grasp](https://github.com/silverback-ventures/grasp), a code review tool for the agent era.

One static file, `index.html`. No build step, no dependencies beyond the Geist fonts loaded from Google Fonts. The colors, type and components follow the Grasp design system: black canvas, white foreground, a gray ramp for hierarchy, and one orange accent for the cursor and the primary action. Light theme follows the OS preference, with a toggle in the header.

## Run it

Open `index.html` in a browser, or serve the directory:

```bash
python3 -m http.server 8000
```

## Deploy

Any static host works. Point it at the repository root.
