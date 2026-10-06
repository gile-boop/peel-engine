# peel-engine

Built sticker engine for the peel. sticker maker, packaged as one classic script that defines `window.Peel`.
Loaded by a Brik tool via jsDelivr. Source lives elsewhere; this repo only holds build output.

Needs, loaded first:
- https://cdn.jsdelivr.net/npm/opentype.js@1.3.4/dist/opentype.min.js
- https://cdn.jsdelivr.net/npm/clipper-lib@6.4.2/clipper.js

```js
await Peel.init();            // fetches fonts (fontsource via jsDelivr)
Peel.useStyle('team');
await Peel.draw(canvas, Peel.fromType('round'));
```
