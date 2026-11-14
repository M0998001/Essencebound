# Essencebound — Lanterns of Calderhal

Playable dark-fantasy browser RPG, based on the **Legacy & Horizons** expansion and the redesigned title screen.

**Play:** https://m0998001.github.io/Essencebound/

## Deployment
The repository's **index.html** loads the complete game from 17 sequentially numbered files in **game/**. The browser downloads them in parallel, reconstructs the original HTML, and launches it at the same URL.

This layout works on GitHub Pages and avoids submitting one 11.6 MB file via constrained publishing integrations. The game parts must be uploaded together; do not reorder or edit them independently. A single-file offline release can still be distributed separately.

A Pages deployment workflow is included in `.github/workflows/pages.yml`. If GitHub requires an initial setup step, open **Settings → Pages** and select **GitHub Actions** as the source.

## Artwork directories
Future game art should live in these locations and be referenced by relative paths:
- `assets/npcs/`
- `assets/enemies/`
- `assets/bosses/`
- `assets/scenes/`
- `assets/ui/`

The initial 14-artwork pilot now supplies six NPC portraits, six enemy combat images, and two boss images. The game loads WebP files on demand using relative paths, such as `assets/npcs/maud.webp`. Missing images are hidden automatically.

## Existing saves
Browser saves are origin-specific. Local saves from `file://` or other hosts will not automatically appear on GitHub Pages. **Export a save code from the earlier game and import it into this edition.**

## Offline play
For fully offline play, use the original `Essencebound_Lanterns_of_Calderhal.html` standalone file or serve this repository with a local HTTP server. The Pages loader uses `fetch`, which may not work when opened directly as `file://`.
