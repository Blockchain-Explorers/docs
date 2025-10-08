# What is this ?

A lightweight template for MkDocs GitHub Pages website that's geared towards building project documentation.

Easily deploy your own themed static website with support for markdown, diagrams and charts. Just like this one.

The template is using [python](https://www.python.org/downloads/), [mkdocs](https://www.mkdocs.org/user-guide/installation/), [mermaid](https://mermaid.js.org/) and [material theme](https://github.com/squidfunk/mkdocs-material) to generate a static website from GitHub flavored markdown.

## How to use

1. Fork this **[repository](https://krko12345.github.io/mkdocs-gh-pages-template/)** into your GitHub organization

2. Clone the forked repository into your local folder

3. Run command `npm install`

    - You must also install `python` if you haven't already

4. Update the content of your site

    - The TITLE and NAVIGATION of your website is stored in the `mkdocs.yml` file.

    - The CONTENT of your website is stored as markdown files in the `/docs` folder.

5. Deploy the updates

    - Push your commits to your `main` branch.

    - Your commits will be automatically processed by the python script and pushed to `gh-pages` branch.

6. Visit your website

    - Your updated website will be automatically available at `https://YOUR_ORGANIZATION.github.io/YOUR_FORKED_REPO/`

</br>

!!!Note
    The websites in GitHub Pages are always available to public audience. Make sure you don't expose any sensitive data in the website content.

</br>
