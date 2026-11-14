# Essencebound

A dark-fantasy RPG playable in your browser. The current edition is **Lanterns of Calderhal**, built on the Legacy & Horizons expansion.

## Play online

Once GitHub Pages is enabled for the `main` branch at the repository root, the game will be available at:

https://m0998001.github.io/Essencebound/

## Hosting

- `index.html` — the complete playable game, including its current title-screen artwork and game data.
- `assets/npcs/` — character portraits for a future visual expansion.
- `assets/enemies/` — enemy artwork.
- `assets/bosses/` — boss illustrations.
- `assets/scenes/` — story backgrounds.
- `assets/ui/` — reusable interface art.

Image references should be relative to this repository root, for example `assets/npcs/maud.webp`, so they work both on GitHub Pages and local servers.

## Important save note

The game uses local browser storage. A save made on another domain or opened directly as a file does not automatically appear on the GitHub Pages website. Export your save code in the previous version, then import it into the hosted edition.

## Setup

In **Settings → Pages**, select **Deploy from a branch**, branch `main`, folder `/(root)`, and save. GitHub Pages deploys the repository root as a static site. No bundler is required.
