---
title: Ultimate 3D Interaction & Tilt Upgrade
type: note
permalink: implementations/ultimate-3-d-interaction-tilt-upgrade
---

Delivered the "Ultimate UI Upgrade" for the docsify blog.
Improvements:
- **3D Birds Background**: Switched from static Net to dynamic `Vanta.js BIRDS`. Birds fly in 3D space and react to mouse clicks and movements.
- **3D Tilt Effect**: Integrated `Vanilla-tilt.js`. Buttons and bookmark cards now tilt in 3D space as the mouse moves over them, including a "glare" effect for a premium plastic/glass feel.
- **Transparency Fix**: Identified that the `docsify-darklight-theme` was overriding the cover background with a solid gradient. Fixed this by setting `coverBackground` and `background` to `transparent` in the theme config.
- **Micro-interactions**: Added sequenced animations for the hero section and refined the typography to be bolder and more impactful.
- **MutationObserver**: Used a `MutationObserver` to ensure tilt effects are applied to dynamically loaded cards even as the user navigates the single-page app.
