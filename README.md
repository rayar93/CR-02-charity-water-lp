# Day One

A browser puzzle game about clean water, built as a game prototype for [charity: water](https://www.charitywater.org/). Rotate pipe tiles to connect a water source to every tap stand on the board before the clock runs out. The name comes from charity: water's own phrase for the first day a community has clean water.

**Play:** https://rayar93.github.io/day-one/

## How it works

The whole game is a single `index.html` with no build step and no dependencies beyond a Google Fonts stylesheet.

**Pipes are bitmasks.** Each tile's openings are a 4-bit mask (N=1, E=2, S=4, W=8), so turning a tile is a bit rotation and two neighbors connect when each has an opening facing the other. After every turn, a breadth-first search from the source finds every tile the water reaches, and each tile's distance from the source sets the delay on its animation.

## Credits and brand

The game was generated with Replit's AI from charity: water's brand guide, as mandated by the Global Career Accelerator assignment it was created for. Every named color comes from the official palette in the guide.

**Day One is a student prototype and is not affiliated with or endorsed by charity: water.** The charity: water name, logo, and quoted figures belong to charity: water and are used here for coursework only.
