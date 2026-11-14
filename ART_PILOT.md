# Essencebound: Character & Encounter Art Pilot (draft branch)

This is a **development branch, not the live game**.

The game code in `game/part-00.txt` and `game/part-16.txt` now optionally renders:
- NPC dialogue portraits: `assets/npcs/{maud,caspian,gannet,anselm,seraphine,ottoline}.webp`
- Enemy combat thumbnails: `assets/enemies/{wolf,shardling,ghoul,cinderknight,spawn,acolyte}.webp`
- Boss combat thumbnails: `assets/bosses/{matriarch,prior}.webp`

Images are optional. Failed loads are hidden so the underlying gameplay remains text-only instead of displaying broken image icons.

**Artwork uploaded:** all 14 optimized WebP image files are now in the repository under the paths above. Git blob SHA-1 checks matched each original asset.

**Suggested post-upload testing:** open a Pages/localhost preview, test Maud dialogue, a Bloom-Wolf encounter and the Glass Matriarch and Ash Prior boss cards on mobile and desktop; test no-network image fallback, save-load, and returning to title. Only merge to `main` after assets are present and tests pass.

No ability/stats/content changes are intended. This is a visual pilot.
