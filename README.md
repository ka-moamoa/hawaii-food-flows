# Hawaii Food Flows

Food and cash grant flows among Hawaii food and agriculture nonprofits, their partner agencies and farms, and the national networks and funders that supply them, reconstructed from IRS Form 990 filings, federal award records and Single Audits, with the state's three statutory food goals and county fact sheets alongside.

Live page: https://ka-moamoa.github.io/hawaii-food-flows/

## Overview

Hawaii Food Flows reconstructs Hawaii's food system from public records alone: IRS filings, federal award data, Single Audits, USDA and Census data, NOAA landings, the state GIS, and the agencies' own reports to the Legislature. It was built for the statewide food systems coordination conversation as a companion to the data-landscape work. Everything drawn from the June 2026 convening is marked draft until the coordination team reviews it.

What it does that nothing else does today:

- **Every recorded grant of food or money** between Hawaii food and agriculture organizations, their partners and their national suppliers, as a network, a Sankey and a map: 848 organizations and 1,281 flows from 603 tax returns, with the audited USDA commodity food each food bank receives drawn in.
- **The first compiled table** of every local-purchasing report the agencies file under Acts 175 and 176, with an owner, a status and the basis each agency measured on, set beside the three statutory goals.
- **School food dollars traced to the seven distributors** that supply them, the first farm-side flows in the record.
- **One fact sheet per county and per state Senate and House district**: household need from the food banks' survey and ALICE, farmland in use by crop, farm sales into local channels, and the organizations located there.
- **The steward inventory as a map**: the 36 organizations the convening documents name as producers, keepers or users of food-system data, and the 41 relationships the documents describe, drawn as an interactive map with the source document on each link, at [/system-map](https://ka-moamoa.github.io/hawaii-food-flows/system-map). A seed for the team to correct through two published spreadsheets.
- **Need beside supply**: Feeding America's Map the Meal Gap county estimates for 2024 (food insecurity rate, children, meal gap, share above the SNAP income line) set against the charitable food the record places in each county, as an upper bound on coverage; the same estimates shade the map by county and can tint the network.
- **Moku, Hawaiian home lands, legislative districts and 886,000 acres of 2020 farmland** as map layers, and every source table downloadable with EIN as the shared identifier.

What it does not do:

- **It does not see farms, hubs or retailers directly.** Form 990 covers nonprofits. Companies and cooperatives appear only where a public record names them, such as the school system's contracted distributors.
- **It does not measure household food security.** The county figures quote the food banks' survey, Aloha United Way's ALICE report and Feeding America's Map the Meal Gap county model as published, each with its label; the site adds no estimate of its own and never computes food per resident.
- **It does not show where food is eaten.** A point is a mailing address; a Honolulu warehouse serves other islands. Flows are drawn as straight lines between addresses, not shipping routes.
- **It does not see grants under $5,000, donors, or anything filed on a 990-EZ or 990-N**, so agencies that appear to have one source may have several small ones, and neighbor-island food banks that itemize few grantees look thinner than they are.
- **It does not rebase the agencies' local-purchasing shares to a common definition.** A 15 percent on produce at one hospital and a 6 percent on all school food are shown side by side with their bases, not made comparable.
- **It does not include a production or self-sufficiency metric**, because none exists; it shows the Census, landings and farmland series that do exist and says what a real measure would need.

One finding to think about: in 2022 Hawaii farms sold $43 million directly to consumers and $187 million directly to local retailers, institutions and food hubs. Together that is about a third of all farm sales, and both channels grew by half since 2017. Meanwhile the state agencies required to buy local sit at 4 to 7 percent of their food budgets. The local marketing economy the purchasing laws are meant to build already exists, mostly on Hawaii Island; the public buyers are the ones not yet in it.


Permalinks: [/network](https://ka-moamoa.github.io/hawaii-food-flows/network), [/sankey](https://ka-moamoa.github.io/hawaii-food-flows/sankey), [/system-map](https://ka-moamoa.github.io/hawaii-food-flows/system-map), [/map](https://ka-moamoa.github.io/hawaii-food-flows/map), [/food-security](https://ka-moamoa.github.io/hawaii-food-flows/food-security), [/goals](https://ka-moamoa.github.io/hawaii-food-flows/goals), [/islands](https://ka-moamoa.github.io/hawaii-food-flows/islands), [/priority-areas](https://ka-moamoa.github.io/hawaii-food-flows/priority-areas), [/about](https://ka-moamoa.github.io/hawaii-food-flows/about). Each route folder holds a copy of the same page; the page reads the route from its path.

This repository holds only the deployed page. The pipeline, source tables and provenance log are in the private repository `ka-moamoa/hawaii-food-flows-990`. The About the data tab on the page documents every source, join, assumption and label.

## Credits

Hawaii Food Flows is a project of the Ka Moamoa lab at the Georgia Institute of Technology, built on the Atlanta Food Flows pipeline and prepared for the Hawaii statewide food systems coordination conversations.

- **Dr. Josiah Hester**, Lab Director, Ka Moamoa

Developed in working sessions with Claude (Anthropic).

## Data

The `data/` folder holds the source tables the page is built from: `data.json` (organizations, flows, federal layers, geography), the organization set, the TEFAP table, the compiled local-purchasing filings, production context, county reference figures, the priority areas, the steward inventory, and `mmg.json`, the harmonized Feeding America Map the Meal Gap series (county and state, 2009 to 2024, with the comparability rules from the 2026 technical brief). The organization identifier is the EIN wherever one exists.
