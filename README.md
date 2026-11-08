# Mở Pack Thẻ Quái Thú (Monster Pack Card Game)

A browser card game in Vietnamese: open booster packs, collect monsters, fuse duplicates, evolve maxed cards, and battle with an elemental counter system. A single self-contained static site - just open `index.html` in a browser, no build step, no backend.

## How to play
- **Open packs** - 100 xu per pack, 5 cards per pack, 20 collectible monsters across 5 rarity tiers (Common 58% / Rare 27% / Epic 10.5% / Legendary 4% / Shiny 0.5%). The last card of every pack is Rare or better, and a pity guarantee kicks in after 9 packs without an Epic.
- **Coin economy** - sell duplicate cards for xu, claim 100 free xu every 20 seconds, earn milestone rewards at 6 / 9 / 12 / 20 unique cards.
- **Fusion (Hợp Thể)** - feed duplicates into a card to raise it up to +5 levels (+15% HP and ATK per level, +75% max). Fused cards are locked from selling.
- **Evolution (Tiến Hóa)** - a max-fused card can evolve for 300 xu into a humanoid form with new art and ×1.6 stats.
- **Card Battle Arena (Đấu Trường Thẻ)** - pick 3 cards from your collection, pay 50 xu to enter, best-of-3 duels. Win 180 xu, lose and still get 20 xu.

## Battle system
- Five-element counter wheel: Metal → Wood → Earth → Water → Fire → Metal (×1.5 damage when strong, ×0.75 when weak)
- Light ⇄ Darkness counter each other both ways (×1.5)
- Special rule - **Chaos vs Clown**: Chaos cards deal ×2 damage to everything, but instantly lose the round if the opposing team contains a Clown anywhere. Clown cards deal 0 damage to every other monster and can only beat Chaos.

## Tech
- Vanilla HTML, CSS, JavaScript in a single `index.html`
- Card art: original AI-generated chibi monster sprite sheets, embedded directly in `index.html` as data URIs (recompressed for the web) and cropped per card with CSS; Shiny variants reuse the art with CSS color filters
- Sound effects synthesized with WebAudio; progress is kept in memory for the session only

---
Built & signed by **NhanDev** · [github.com/doanquocnhan](https://github.com/doanquocnhan)
