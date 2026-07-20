# Flower Bouquet

An interactive digital flower bouquet garden built with vanilla HTML5 Canvas, CSS, and JavaScript. The page populates with blooming flowers, a GPU-accelerated ambient glowing background, and support for URL-customized greetings.

## Quick Links

- Live Site: [bouquet.745482.xyz](https://bouquet.745482.xyz)
- Custom Link Creator: [bouquet.745482.xyz/create](https://bouquet.745482.xyz/create)
- Live Preset Demo: [bouquet.745482.xyz/?love](https://bouquet.745482.xyz/?love)

## Core Interactions

- **Interactive Sway Physics:** Flowers are simulated with a second-order spring-mass-damper system. Moving the mouse generates wind that pushes the flowers away, scaling dynamically with mouse velocity.
- **Mobile Parallax and Motion:** Tilting the device sways the flowers collectively from their base points. Shaking the device triggers temporary wind gusts proportional to dynamic acceleration.
- **Constant Ambient Breeze:** A multi-frequency background wave keeps the garden continuously swaying when idle.
- **Procedural 24-Hour Sky Engine:** Real-time sun arc, real-date 8-phase lunar cycle, twinkling star field, drifting parallax clouds, atmospheric horizon mist, and 24-hour ambient lighting keyframes synchronized with local time.
- **Ambient Sound Scapes:** Integrated multi-channel audio player featuring relaxing ambient soundscapes (rain, ocean waves, fireplace).
- **Draggable Glass Windows & Dock:** Interactive bottom glass dock toolbar and draggable, resizable floating window system for managing tools and soundscapes.
- **Live Local Clock:** Real-time clock display seamlessly integrated into the garden background.

## Customization and Presets

You can pass query parameters to customize the text, typography, count, and theme:

- **Custom message:** `?text=Your+Message`
- **Presets:** `?birthday`, `?love`, `?exam`, `?sorry`, `?getwell`, `?thankyou`, or `?cheer`.
- **Garden controls:** `?count=15`, `?flower=rose`, `?grow=10&unit=sec`, `?bg=night`, `?hour=19.5`.
- **Typography:** Append `&font=mono` to use JetBrains Mono (defaults to Inter sans-serif).

For an interactive link builder UI, visit the creator page at `/create/`.

## File Structure

- `index.html` - Main page entry point and metadata.
- `style.css` - Primary layout styles, UI components, and typography.
- `script.js` - Main animation loop, spring physics solver, and procedural flower rendering.
- `background.js` - Procedural 24-hour sky module (sun, moon phases, stars, clouds, ambient light keyframes).
- `floating-window.js` - Reusable draggable and resizable glass window manager.
- `dock.js` & `dock.css` - Interactive bottom navigation glass dock toolbar and styling.
- `ambient-sounds.js` - Multi-channel ambient audio player engine.
- `create/` - Interactive bouquet link creator tool (`index.html`, `script.js`, `style.css`).
