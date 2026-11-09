# thermal-system-app

## Claude analysis (2026-11-09)

This section was written by Claude (an AI assistant) after reading the repository. It has not been reviewed by a person.

**What it is:** a single-file web page (`index.html`, about 560 lines, no build step) titled "Thermal System 3D Schematic & Analysis". It shows a hybrid thermal management system for a five-platen press and estimates the cost and payback of adding it.

**What it contains**
- A 3D schematic drawn with Three.js (r128, loaded from a CDN). It has five platens with internal loops, manifolds, a heat exchanger, unit heaters, an existing gas oil heater, and four labelled valves. The view can be rotated.
- A Winter and a Summer mode button that change how recovered heat is routed.
- Editable electricity and natural gas prices.
- Tables for capital cost (CapEx), annual operating cost (OpEx), recovered-heat savings, and a payback figure. A print button produces a report.

**How it works:** the page recalculates the tables from the two price inputs and a set of fixed constants written in the script (energy use per item, recovered heat, gas efficiency, capital cost, maintenance). The constants are hard-coded and have no sources recorded in the repo.

**Status:** one commit (2026-04-23), one file, no README before this analysis. Nothing in the repo says who the figures were prepared for or whether the constants are measured or estimated. Treat the numbers as unverified.

**Note:** this repo is public and the page contains facility-specific cost figures. If those are not meant to be public, make the repo private.
