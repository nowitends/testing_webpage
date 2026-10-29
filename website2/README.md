# Chile Field Guide — MkDocs

This folder is the MkDocs version of the Chile research portal. Its Markdown
pages are in `docs/`; the single-file website remains in the sibling `website/`
folder.

## Run locally on Windows

Open PowerShell in the repository root and run:

```powershell
py -m venv .venv
.\.venv\Scripts\Activate.ps1
python -m pip install -r website2\requirements.txt
python -m mkdocs serve --config-file website2\mkdocs.yml
```

Open the local address printed by MkDocs, normally
<http://127.0.0.1:8000/>. Stop the local server with **Ctrl+C**.

To build the static site without starting a server:

```powershell
python -m mkdocs build --strict --config-file website2\mkdocs.yml
```

The generated site is written to `website2/site/`. This generated output is
temporary and should not be edited by hand.

## Publish on GitHub Pages

The repository's **Deploy website** GitHub Actions workflow builds this MkDocs
project and publishes it to <https://nowitends.github.io/testing_webpage/>.
The existing single-file site remains available at
<https://nowitends.github.io/testing_webpage/website/>.

Push changes to `website2/`, `website/`, or the deployment workflow on `main`
to trigger a new deployment. Make sure the repository's Pages source is set to
**GitHub Actions** in **Settings → Pages**.

## Update portal content

Edit the relevant Markdown page in `docs/`, then preview it with `mkdocs serve`.
Navigation and site metadata are configured in `mkdocs.yml`. The repository's
original research notes remain at the repository root; the copies in `docs/`
are the pages used by this MkDocs portal.
