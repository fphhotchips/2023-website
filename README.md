# PyConline AU 2020 website

To build this website, you will need the following:

- **Python 3.7** installed and activated.
- **Node.js** and **Yarn** installed.
- **Poetry** installed; see [the installation documentation](https://python-poetry.org/docs/#installation).

Then:

- Run `poetry install`. Poetry will create a virtualenv for you.
- Run `yarn install`.
- Run `poetry run supervisord`. Supervisor will start up the two processes you'll need for local development: `parcel` (to build frontend static assets) and `statik` (to build the site itself).

From there, the [Statik documentation](https://github.com/thanethomson/statik/wiki) will be the place to look for most things.

Deployment is automated, and runs on Netlify; see the `netlify.toml` for details.