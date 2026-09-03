# cogniti DESIGN.md

> Auto-generated design system — reverse-engineered via static analysis by skillui.
> Frameworks: None detected
> Colors: 13 · Fonts: 2 · Components: 0
> Icon library: not detected · State: not detected
> Primary theme: dark · Dark mode toggle: no · Motion: none

## Visual Theme & Atmosphere

Dark-themed interface with a cool tone. Depth is expressed through layered shadows and subtle surface colour variation. The implementation resolves the source specification's typography inconsistency in favour of the repeated rule: **Jost for display/headings and Arial for body/UI text**. Spacing follows a 5px base grid.

## Colour Palette

- background `#2b2b2b`
- surface `#000000`
- text-primary `#ffffff`
- text-muted `#566e8b`
- border `#595959`
- accent `#24cc8f`
- success `#00b682`
- warning `#fcaf3b`
- info `#528ffe`
- near-black `#121212`
- light `#ededed`
- charcoal `#32373c`
- soft `#d2d4d1`

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
- Card surface: `#000000`
- Card border: 1px solid `#595959`
- Card radius: 7px
- Card padding: 20–25px
- Primary button: `#24cc8f`, black text, 10px 20px padding, 7px radius
- Focus ring: 2px `#24cc8f`
- No gradients, blur or backdrop blur

## Elevation

- Raised: `rgba(0, 0, 0, 0.1) 0px -1px 3px 0px`
- Raised: `rgba(0, 0, 0, 0.1) 0px 3px 6px -5px, rgba(0, 0, 0, 0.1) 0px 4px 8px 0px`
- Overlay: `rgba(40, 47, 98, 0.08) 0px 10px 100px 0px`

## Responsive Behaviour

Mobile-first fallbacks are provided at 900px and 650px. Three-column agent cards collapse to two columns and then one column. Detail layouts similarly collapse to a single column on small screens.