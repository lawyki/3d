# 3d

Working space for the 3D web pieces built in the "3D projects" project. Every piece is one self-contained HTML page with no build step. Some load three.js 0.160 from unpkg; the rest are raw WebGL. Screenshots sit in each piece's `stills/` folder.

## Viewing

```sh
git clone https://github.com/lawyki/3d && cd 3d
python3 -m http.server 8000
# open http://localhost:8000/<piece>/  e.g. http://localhost:8000/vare/
```

Opening `index.html` straight from disk works for most pieces too. A desktop browser with a decent GPU gives the intended frame rate. Pieces are made-up brands and places unless noted.

## Pieces

Newest first, roughly.

| Piece | What it is |
|---|---|
| [vare](vare/) | Väre: a sea-pool site laid in tile on a pool floor under refracting water with caustics; drag the lifebuoy to set the time of day. `src.html` is the same page with font placeholders. |
| [planetary-gearbox](planetary-gearbox/) | Blender renders and an animation of a planetary gearbox (not a web page). |
| [keha](keha/) | Kehä K116: a scroll page that takes apart a working robot joint actuator with real involute planetary gears, motor and crossed-roller bearing. |
| [nivel](nivel/) | Nivel J120: robot joint actuator product page with real gear kinematics, section cuts and an exploded view. |
| [laskos](laskos/) | Laskos: paper mill site where the page is one pleated sheet with a page printed on each pleat face. |
| [untu](untu/) | Untu: down quilt page that is itself a sewn, inflated quilt; the layout is the seams. |
| [hieta](hieta/) | Hieta: guesthouse page lying on raked sand, where type is grains and text blocks are stones. |
| [loose-matter](loose-matter/) | Loose Matter: sand page where type and layout are sculpted from one grain bed and DOM text shares its 3D plane. |
| [jyva](jyva/) | Jyvä: a bed of sand printed into objects layer by layer. |
| [vire](vire/) | Vire: a playable 400-string instrument whose shape is its tuning. |
| [kierre](kierre/) | Kierre 27: conference page with one kinetic sculpture of 150 metal blades that re-forms per section. |
| [strand](strand/) | Strand Line One: a scroll ride up a space lift from the sea to orbit. |
| [tyyni](tyyni/) | Tyyni: single-screen lamp product page with a live 3D configurator. |
| [aukko](aukko/) | Aukko: ray-marched concrete light pavilion you walk through by scrolling. |
| [microscope](microscope/) | Diatom Microscope: scroll film following the light path through a microscope, on the Flint Prism tracer. |
| [prism](prism/) | Flint Prism: one physically exact prism where particles meet glass without clipping. |
| [ydt-grain](ydt-grain/) | The site of YDT Holdings Oy (a real company) drawn in the Kaiku Dust grain style. |
| [kaiku-dust](kaiku-dust/) | Kaiku Dust: one point cloud of soft grains morphing between sampled forms; the grain style to reuse. |
| [kaiku-ball](kaiku-ball/) | Kaiku Ball: only the hero ball from Kaiku, a sphere of dust that breathes and rings when clicked. |
| [lyse](lyse/) | Lyse: light film of rays of beads through glass elements, the smooth follow-up to Sillage. |
| [sillage](sillage/) | Sillage: particle-and-glass perfume film site. |
| [halden](halden/) | Halden: scroll film of a made-up watch that opens onto a running movement. |
| [kaiku](kaiku/) | Kaiku: scrolling site for an acoustics studio; 110,000 grains take a new form per section. |
| [vuorokausi](vuorokausi/) | Vuorokausi: scroll film through a generated northern landscape from first light to the northern lights. |
| [mercury](mercury/) | Mercury: ten ray-marched drops of liquid metal that merge into one surface. |
| [drape](drape/) | Drape: real-time cloth simulation of 6,561 points over a sphere. |
| [three-free-things](three-free-things/) | Poured C (glass tube), Helix (B-DNA to scale from a typed sequence) and 126 (a bar floor rippling at 126 BPM). |

## Contributing

Open work is tracked in [issues](https://github.com/lawyki/3d/issues); ones marked `good first issue` need no WebGL background. See [CONTRIBUTING.md](CONTRIBUTING.md) for how the repo is laid out and how to send a change.

## License

Two licenses, split by what you are reusing:

- **Code** (HTML, CSS, JavaScript, shaders): [MIT](LICENSE-MIT). Take a technique, a shader or a whole page's code and use it anywhere, with credit.
- **Visual work** (the pages as designed works, their copy and made-up brands, every `stills/` screenshot, and the `planetary-gearbox/` renders and video): [CC BY-NC 4.0](LICENSE-CC-BY-NC-4.0). Share and adapt with credit, not for commercial use.

Details and third-party exceptions are in [LICENSE](LICENSE). Contributions are accepted under the same terms.
