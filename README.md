# 3d

Small 3D experiments. Open `index.html` in a browser; there is no build step.

## Three free things

One page, three scenes, switched from the top bar:

- **Poured C** (`#glass`): Clara's C as a glass tube with the brand pour running through it. Sliders for fill and frost.
- **Helix** (`#helix`): type a DNA sequence and get B-DNA drawn to textbook scale (10.5 base pairs per turn, 0.34 nm rise), with the complementary strand, GC share, hydrogen bonds and the translated protein.
- **126** (`#pulse`): a floor of 1,600 bars that ripples at 126 BPM, with an optional G♯ minor synth made in the browser.

Drag to turn a scene, scroll to zoom. Built with three.js 0.160 loaded from unpkg.

## Drape

`drape/index.html` is a real-time cloth simulation: 6,561 points joined by 38,558 threads, held by its corners over a sphere. Drag the cloth to pull it, press Let go to drop it, Lift to pick it back up.

## Mercury

`mercury/index.html` is ten drops of liquid metal that merge into one surface. Press and hold to pull them toward the pointer, let go and they fall and pool. It uses no library: the picture is ray-marched in a fragment shader, so there are no polygons.

## Vuorokausi

`vuorokausi/index.html` is a scroll-driven film through a generated northern landscape: five scenes from first light to the northern lights, each with its own palette, sun and camera position. The land, forest, sea and sky are ray-marched in one fragment shader with no library.

## Kaiku

`kaiku/index.html` is a complete scrolling site for a made-up acoustics studio. One cloud of 110,000 grains sits behind the page and takes a new form per section: a ringing sphere, sand on a vibrating plate (pick the mode), two interfering waves, a cochlea, and the wordmark. No library; the grains are moved in a vertex shader.

## Halden

`halden/index.html` is a product page for a made-up hand-wound watch movement. The movement is built from code (plate, barrel, spoked gear train, escapement, balance with hairspring, striped bridges, rubies, blued screws) and runs at true tooth ratios. Scrolling takes it apart by layer with callouts, moves in on the escapement, shows the train from above and puts it back together. Uses three.js.
