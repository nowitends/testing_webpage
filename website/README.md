# Chile website

This is a self-contained static website. It is a single `index.html` file and
does not need a framework, package installation, build command, or external
assets.

## View it on your computer

1. Open `index.html` in a web browser. You can also double-click the file.
2. The page and its place filters work without an internet connection. Source
   links need an internet connection.

## Share it on the internet with GitHub Pages

This repository includes a GitHub Actions workflow that publishes only the
`website` folder. The repository is public, so the finished page will be
available to everyone with a browser.

1. Push the `website` folder and `.github/workflows/deploy-website.yml` to the
   repository's `main` branch.
2. On GitHub, open the repository and go to **Settings → Pages**.
3. Under **Build and deployment**, set **Source** to **GitHub Actions**.
4. Open the **Actions** tab and select **Deploy website**. If the workflow has
   not started, select **Run workflow** and choose the `main` branch.
5. Wait for the deployment run to finish successfully. The public website URL
   is <https://nowitends.github.io/testing_webpage/>.

After setup, each push that changes `website/` automatically republishes the
site. You can also start a deployment from the **Actions** tab. If the workflow
ran before Pages was enabled and failed, enable Pages as above, then rerun the
workflow.

You can also publish the `website` folder using another static web host: select
`website` as the publish directory and share the public URL provided by that
host. Do not share the local file path; it only works on your computer.

## Updating the site

Edit `index.html`, save it, and reload the page. The source notes are in the
Markdown files in the repository; update the corresponding website content when
those figures or descriptions change. Census figures are specifically labeled
as enumerated 2024 data. Place coordinates are approximate.

This is a plain HTML site, not a MkDocs project. MkDocs can be explored later as
a separate way to publish the Markdown documentation.
