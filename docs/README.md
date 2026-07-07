# SolarPill32 pinout configurator

Self-contained interactive HTML page: IDC pin layouts for all 5 headers, with
checkboxes to toggle alternate peripheral functions per pin group. Conflicting
selections (two peripherals wanting the same physical pin) are highlighted
live on the ribbon diagram and pin table.

No build step, no dependencies — `index.html` is the whole page (fonts are
inlined as base64). Open it directly in a browser, or serve this folder
(e.g. via GitHub Pages) as-is.
