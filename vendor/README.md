Local browser dependencies for the AR test, with upstream licenses retained.

- MindAR 1.2.5: npm package mind-ar@1.2.5. Image compiler/controller and Three integration only.
- Three.js: copied from the project's installed 0.185.1 package.
- Compatibility changes in mindar-image-three.prod.js: resolve Three/CSS3D imports locally; replace removed sRGBEncoding import with legacy constant (the AR page explicitly sets outputColorSpace); retain bound resize handler for cleanup.
- CSS3DRenderer resolves Three locally.

No external CDN is required. Regenerate these copies deliberately when upgrading.
