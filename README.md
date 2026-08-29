## Adding a Recipe Repository

The beer inventory on the website is populated automatically by the [Sync Beer Inventory](.github/workflows/sync-beers.yml) workflow. It discovers any repository in the [`allsaintsfermentery`](https://github.com/allsaintsfermentery) organization that has the `recipe` topic and reads its `beer.yml` file.

To add a new beer to the website:

1. Clone or use the [`allsaintsfermentery/recipe`](https://github.com/allsaintsfermentery/recipe) template repository as a starting point for the new recipe repository.
2. Create a new repository in the `allsaintsfermentery` organization.
3. Add the `recipe` topic to the repository (Settings → Topics).
4. Add a `beer.yml` file at the root of the repository following the schema in [`beer.yml.example`](beer.yml.example).

The workflow runs daily and can also be triggered manually from the [Actions tab](../../actions/workflows/sync-beers.yml).
