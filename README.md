> We brew for the greater glory of God and in honor of all His faithful saints.

All Saints Fermentery was established in 2025 to honor the saints who dedicated their lives to God and to enrich Catholic traditions, particularly during feast days, through celebratory beverages.

We take pride in developing each recipe to produce high-quality beers intended for sharing during meals, celebrations, or other significant occasions.

We encourage you to visit this page regularly for updates regarding our brewing schedule and forthcoming releases.

> Omnes Sancti et Sanctae Dei, orate pro nobis.

## Adding a Recipe Repository

The beer inventory on the website is populated automatically by the [Sync Beer Inventory](.github/workflows/sync-beers.yml) workflow. It discovers any repository in the [`allsaintsfermentery`](https://github.com/allsaintsfermentery) organization that has the `recipe` topic and reads its `beer.yml` file.

To add a new beer to the website:

1. Clone or use the [`allsaintsfermentery/recipe`](https://github.com/allsaintsfermentery/recipe) template repository as a starting point for the new recipe repository.
2. Create a new repository in the `allsaintsfermentery` organization.
3. Add the `recipe` topic to the repository (Settings → Topics).
4. Add a `beer.yml` file at the root of the repository following the schema in [`beer.yml.example`](beer.yml.example).

The workflow runs daily and can also be triggered manually from the [Actions tab](../../actions/workflows/sync-beers.yml).
