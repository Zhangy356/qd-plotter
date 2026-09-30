# QD Data Plotter

A single-page web app for plotting and exporting measurement data from Quantum Design instruments.

**Open it:** https://zhangy356.github.io/qd-plotter/

## What it does

- Opens `.dat` files from DynaCool / PPMS resistivity, heat capacity and MPMS3 and detects the file type automatically.
- Plots any column against any other, with stacked subplots that share the x axis and several curves per subplot.
- Adds calculated columns: time in minutes, resistivity and R/R(300 K) for resistivity; 1/T and molar susceptibility for MPMS3; molar C, C/T and T² for heat capacity. Sample dimensions, formula and mass go in the "Sample inputs" panel.
- Filters rows by column ranges.
- Exports the chosen columns (including calculated ones) to CSV.
- Styles figures for publication: closed frame, inward ticks, log or linear axes, Arial labels, colored curve labels instead of a legend.

Everything runs in your browser. Files you open are read locally and are never uploaded anywhere.

## Running it offline

Download or clone this repository and open `index.html` in a browser. Plotly and the fonts are in `vendor/`, so no internet connection is needed.
