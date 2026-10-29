# Chile website

This is a self-contained static website. It is a single `index.html` file and
does not need a framework, package installation, build command, or external
assets.

## View it on your computer

1. Open `index.html` in a web browser. You can also double-click the file.
2. The page and its place filters work without an internet connection. Source
   links need an internet connection.

## Share it on the internet with GitHub Pages

This repository includes a GitHub Actions workflow that publishes the MkDocs
portal from `website2/`. The repository is public, so the finished page is
available to everyone with a browser. This single-file website remains
available at <https://nowitends.github.io/testing_webpage/website/>.

1. Push the `website2/` folder and `.github/workflows/deploy-website.yml` to
   the repository's `main` branch.
2. The **Deploy website** workflow builds the MkDocs project and publishes it
   to <https://nowitends.github.io/testing_webpage/>.
3. If the workflow has not started, open the **Actions** tab, select
   **Deploy website**, and choose **Run workflow** for the `main` branch.
4. Wait for the deployment run to finish successfully.

The repository's Pages source must be set to **GitHub Actions** under
**Settings → Pages**. Each push that changes `website/`, `website2/`, or the
deployment workflow automatically republishes both sites. The single-file
version is included under the `/website/` path.

You can also publish the `website` folder using another static web host: select
`website` as the publish directory and share the public URL provided by that
host. Do not share the local file path; it only works on your computer.

## Updating the single-file site

Edit `index.html`, save it, and reload the page. The source notes are in the
Markdown files in the repository; update the corresponding website content when
those figures or descriptions change. Census figures are specifically labeled
as enumerated 2024 data. Place coordinates are approximate.

For the MkDocs portal, see [the website2 setup guide](../website2/README.md).
