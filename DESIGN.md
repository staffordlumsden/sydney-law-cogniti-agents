# cogniti DESIGN.md

> Auto-generated design system — reverse-engineered via static analysis by skillui.
> Frameworks: None detected
> Colors: 13 · Fonts: 2 · Components: 0
> Icon library: not detected · State: not detected
> Primary theme: light · Dark mode toggle: yes · Motion: none

## Visual Theme & Atmosphere

Light mode is the default interface, with the original cool dark theme available through a persistent header toggle. Depth is expressed through layered shadows and subtle surface colour variation. The implementation resolves the source specification's typography inconsistency in favour of the repeated rule: **Jost for display/headings and Arial for body/UI text**. Spacing follows a 5px base grid.

## Colour Palette

### Light mode — default

- background `#ededed`
- surface `#ffffff`
- text-primary `#121212`
- text-secondary `#32373c`
- text-muted `#566e8b`
- border `#d2d4d1`
- accent `#24cc8f`
- success `#00b682`
- warning `#ab641d`
- info `#528ffe`

### Dark mode

- background `#2b2b2b`
- surface `#000000`
- text-primary `#ffffff`
- text-secondary `#d2d4d1`
- text-muted `#566e8b`
- border `#595959`
- accent `#24cc8f`
- success `#00b682`
- warning `#fcaf3b`
- info `#528ffe`
- header/subtle surface `#121212`
- chip surface `#32373c`

## Typography

- Display/headings: Jost
- Body/UI: Arial
- H1: 48px / 700
- H2: 32px / 600
- H3: 24px / 600
- Body: 16px / 400
- Caption: 12px / 400

## Layout & Components

- Max width: 1280px
- Base grid: 5px
- Card surface: `#ffffff` in light mode / `#000000` in dark mode
- Card border: 1px solid `#d2d4d1` in light mode / `#595959` in dark mode
- Card radius: 7px
- Card padding: 20–25px
- Primary button: `#24cc8f`, black text, 10px 20px padding, 7px radius
- Focus ring: 2px `#24cc8f`
- Theme toggle: persistent light/dark control in the header; light mode is the first-visit default
- No gradients, blur or backdrop blur

## Elevation

- Raised: `rgba(0, 0, 0, 0.1) 0px -1px 3px 0px`
- Raised: `rgba(0, 0, 0, 0.1) 0px 3px 6px -5px, rgba(0, 0, 0, 0.1) 0px 4px 8px 0px`
- Overlay: `rgba(40, 47, 98, 0.08) 0px 10px 100px 0px`

## Responsive Behaviour

Mobile-first fallbacks are provided at 900px and 650px. Three-column agent cards collapse to two columns and then one column. Detail layouts similarly collapse to a single column on small screens.