# GitHub Pages MkDocs Template

This repository is a reusable lightweight template for GitHub Pages MkDocs website with markdown support.

This template is using [python](https://www.python.org/downloads/), [mkdocs](https://www.mkdocs.org/user-guide/installation/), [mermaid](https://mermaid.js.org/) and [material theme](https://github.com/squidfunk/mkdocs-material) to generate a static website from GitHub flavored markdown.

</br>

## How to use

### 1. Fork the repository to your organization

### 2. Clone forked repository into your local folder

### 3. Run command `npm install`

> You must also install `python` if you haven't already

### 4. Update the content of your site

> The TITLE and NAVIGATION of your website is stored in the `mkdocs.yml` file.</br>
> The CONTENT of your pages is stored in markdown files in the `docs` folder.

### 5. Deploy the updates

> Push your commits to your `main` branch.</br>
> Your commits will be automatically transformed by the post-commit hook and pushed to `gh-pages` branch.

### 6. Visit your website

> Your website will be automatically available at `https://pages.github.ibm.com/YOUR_ORGANIZATION/YOUR_FORKED_REPO`

> The websites in GitHub Pages are always available to public audience. Make sure you don't expose any sensitive data in the website content.

</br>

## Local development

For local usage/development use these command:

```bash
npm install
npm run dev
```

You local site will be available here [127.0.0.1:8000](127.0.0.1:8000)

When creating or updating the content of the local site, `mkdocs` will be used to serve the site locally, and the site will be automatically rebuilt by `mkdocs` as changes are made. The commands below will build and serve the site from a local directory.
