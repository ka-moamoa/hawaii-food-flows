# Hawaii Food Flows

Food and cash grant flows among Hawaii food and agriculture nonprofits, their partner agencies and farms, and the national networks and funders that supply them, reconstructed from IRS Form 990 filings, federal award records and Single Audits, with the state's three statutory food goals and county fact sheets alongside.

Live page: https://ka-moamoa.github.io/hawaii-food-flows/

Permalinks: [/network](https://ka-moamoa.github.io/hawaii-food-flows/network), [/sankey](https://ka-moamoa.github.io/hawaii-food-flows/sankey), [/map](https://ka-moamoa.github.io/hawaii-food-flows/map), [/food-security](https://ka-moamoa.github.io/hawaii-food-flows/food-security), [/goals](https://ka-moamoa.github.io/hawaii-food-flows/goals), [/islands](https://ka-moamoa.github.io/hawaii-food-flows/islands), [/priority-areas](https://ka-moamoa.github.io/hawaii-food-flows/priority-areas), [/about](https://ka-moamoa.github.io/hawaii-food-flows/about). Each route folder holds a copy of the same page; the page reads the route from its path.

This repository holds only the deployed page. The pipeline, source tables and provenance log are in the private repository `ka-moamoa/hawaii-food-flows-990`. The About the data tab on the page documents every source, join, assumption and label.

## Credits

Hawaii Food Flows is a project of the Ka Moamoa lab at the Georgia Institute of Technology, built on the Atlanta Food Flows pipeline and prepared for the Hawaii statewide food systems coordination conversations.

- **Dr. Josiah Hester**, Lab Director, Ka Moamoa

Developed in working sessions with Claude (Anthropic).

## Data

The `data/` folder holds the source tables the page is built from: `data.json` (organizations, flows, federal layers, geography), the organization set, the TEFAP table, the compiled local-purchasing filings, production context, county reference figures, the priority areas and the steward inventory. The organization identifier is the EIN wherever one exists.
