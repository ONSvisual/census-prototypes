# Census 2021 Product Prototypes
This is a summary of the various prototypes that are being developed by the ONS data vis/journalism team for Census 2021.

## Core products
These are the main products that we intend to release in some for in time for publication of Census 2021 data. The links below are to the most recent prototypes. URLs are likely to change.
* **[Census atlas](https://onsvisual.github.io/census-atlas)** - Explore geographic patterns in data down to a small area level.
* **[Area reports](https://theojolliffe.github.io/area-reports/)** - 'Robo-journalism' reports highlighing significant changes in an area between censuses. See also this [earlier demo](https://bothness.github.io/census-robo-v1/).
* **[Area explorer](https://bothness.github.io/area-explorer)** - Navigate through geographic hierarchies and see population data with change from previous census.
* **[Sub-population explorer](https://bothness.github.io/sub-profile)** - Select a sub-population group and see how it compares to others (relies on Cantabular API). See also this [earlier demo](https://bothness.github.io/sub-pop/).
* **[Draw your geography](https://onsvisual.github.io/geo-draw)** - Draw a custom geography and get data, lookups and boundaries (relies on Nomis API and ONS Geography Linked Data).
* **[Build an area profile](https://bothness.github.io/build-profile)** - Build an embeddable/downloadable mini-area profile. Select an area and select datasets.

## Libraries
These are the shared libraries of components and templates that will support the above products as well as other releases.
* **[Scrollytelling template](https://onsvisual.github.io/svelte-scrolly)** - Rich media template with scrollytelling functionality. See also proof-of-concept for importing ArchiML.
* **[Chart component library](https://onsvisual.github.io/svelte-charts)** - Chart components built in Svelte. Can be imported [via NPM](https://svelte.dev/repl/324b696de5304ceebbe0213511e7ed23?version=3.44.0) or used [in vanilla JS](https://codepen.io/bothness/pen/RwVJvav).
* **Map component library** - Not online yet. Example map components can be [found here](https://svelte.dev/repl/ceadf2f8288a4feabb933837f9a4d553?version=3.44.0).
* **UI component library** - Not online yet. Some examples can be found [here](https://svelte.dev/repl/6567a57c08774491b523a34345f8e279?version=3.44.0) and [here](https://svelte.dev/repl/26a3c06475264c6d8917d57bab1174c9?version=3.44.0) (and also within other demos).
* **Census data over time pipeline** - Not online yet. Python scripts for aggregating consistent data across censuses. Sample data [here](https://github.com/onsvisual/census-data-v2).

## In the Wild
Published ONS releases building on the various prototypes and code in development for Census 2021.
* **[COVID-19 restrictions cut household emissions](https://www.ons.gov.uk/economy/environmentalaccounts/articles/covid19restrictionscuthouseholdemissions/2021-09-21)** - Carbon emissions calculator coded in Svelte and embedded in a static article.
* **[Exploring local income deprivation](https://www.ons.gov.uk/visualisations/dvc1371/)** - Scrollytelling article with dynamic maps and localisation using basic robo-journalism techniques (source code available here).
* **[Regional differences in income and productivity](https://www.ons.gov.uk/visualisations/dvc1370/)** - Scrollytelling article with dynamic maps and charts.
* **[Jobs seeing a drop in pay during the pandemic](https://www.ons.gov.uk/visualisations/dvc1227/)** - Scrollytelling with dynamic charts.

## Other demos
### Mapping examples
* **[Dot density mapping](https://powerful-sea-44758.herokuapp.com/)** - Mapping categorical data. See also [calculating dot positions](https://observablehq.com/@jtrim-ons/dot-density-map-a-tweaked-version) + earlier [vanilla JS demo](https://bothness.github.io/census-dots/).
* **[Historic map layers](https://bothness.github.io/ons-basemaps/)** - 
* **[3D Population density](https://bothness.github.io/census-pop-hex/)** - DeckGL example. 3D hex map based on output area data.
* **[Multiply layer blend](https://svelte.dev/repl/63d10e8746c94dea80b86fe5c63c44d7?version=3.44.0)** - Using overlaid + synced Mapbox maps to achieve "multiply" layer blend effect.
* **[Raster masking](https://svelte.dev/repl/0f273e9befba4607a5d5538de9294409?version=3.44.0)** - Masking choropleth area maps using a raster buildings mask layer (an alternative approach to dasymetric mapping with potential to reduce data and improve performance).

### Charts
* **[Animated scatter plot](https://bothness.github.io/imd-scatter/)** - Example using Layer Cake and REGL to animate 10,000s of points with WebGL.
* **[Accurate beeswarm plots](https://observablehq.com/@jtrim-ons/beeswarm-methods-compared)** - Algorithm for calculating accurate + compact beeswarm plots.
* **[Waffle chart](https://svelte.dev/repl/093999ee2ae545feb3aa1ac0625faae2)** - Simple HTML + CSS based waffle chart suitable for pre-rendering (requires CSS Grid support).
* **[Histogram chart](https://svelte.dev/repl/ca5d9b7c2700402aa976d86b14a9613c?version=3.44.0)** - Chart for summarising small area data (used in an earlier version of "census atlas").

### Place search
* **[Simple postcode API](https://observablehq.com/@jtrim-ons/simple-postcode-api)** - A postcode > geography search based on flat file chunks from the National Statistics Postcode Lookup.
* **[Combined postcode + area search](https://svelte.dev/repl/9ef25d3476de462b82600137e2ce91d1?version=3.44.0)** - Get a geography from a predefined list or postcodes.io search depending on query. Also uses a Topojson file to figure out which 1961 district a postcode long/lat falls within.
* **[OS API search](https://svelte.dev/repl/62c68fc0484747ec9b9ec93164c55d20?version=3.44.0)** - Test for getting geographic data for postcodes, streets and cities/towns/villages from the Ordnance Survey Open Names API.

### Games and quizzes
* **How well do you know your area?** - Not online yet. Very basic demo [here](https://svelte.dev/repl/1de9e72b80c44ddda2e10c5cdbed5799?version=3.44.0).
* **[Guess the geography](https://bothness.github.io/ons-geo-game/)** - Guess the name of an area based on a boundary on a map (relies on ONS Geography Linked Data API).
* **[Census fake data quiz](https://bothness.github.io/census-quiz/)** - Guess which characteristic three areas have in common.

### Origin-destination data
* **[Travel to work by MSOA](https://bothness.github.io/census-livework/)** - Find the communtes in and out of an MSOA by postcode or clicking map.
* **[Manchester travel to work](https://bothness.github.io/census-commutes/)** - DeckGL example. Mapping all travel to work in Manchester by mode of transportation.

## Data repositories
Repositories with data and assets used by the above prototypes and demos.
* **[Census data over time](https://github.com/onsvisual/census-data-v2)** - 2001 and 2011 data used by "area explorer" and other core products, above.
* **[ONS basemap styles](https://github.com/bothness/ons-basemaps/tree/master/data)** - A selection of base map styles for use in Mapbox/Maplibre GL JS.
* **[Map tiles for testing](https://github.com/bothness/map-tiles)** - Vector and raster map tiles for use in testing. Not suitable for use in live projects.
