# Example Single FDC3 Repository and Website

Website: https://rikoe.github.io/FDC3

This repository demonstrates using [Docusaurus](https://docusaurus.io) to author and host the FDC3 website and documentation, based on markdown files.

## Plan

- [x] Try out Docusaurus
- [x] Host on GitHub Pages
- [ ] Attempt to apply styling and assets from https://fdc3.finos.org to this website
- [ ] Copy content from other FDC3 repositories into this single repository, to try and achieve a unified structure with an overview, that distinguishes clearly between specifications, examples and usage documentation
- [ ] Apply versioning
- [ ] Add documentation content

## References

FINOS FDC3 [Launch plan] (https://finosfoundation.atlassian.net/wiki/spaces/FDC3/pages/711950361/FDC3+1.0+Release+Public+Launch+Documentation+Sub-Plan)

## Developer Information

The included example website was generated by following the [Docusaurus installation steps](https://docusaurus.io/docs/en/installation).

### Required tools

* NodeJS 8+ [[Install](https://nodejs.org/en/download/)]
* Yarn 1.5+ [[Install](https://yarnpkg.com/lang/en/docs/install/)]
* Docker [[Install](https://www.docker.com/get-started)] (for running locally)

### Structure

The repository follows the standard Docusaurus website structure. For more information, see [Creating your site](https://docusaurus.io/docs/en/site-creation).

```
root-directory
├── docs
└── website
    ├── blog
    ├── core
    │   └── Footer.js
    ├── package.json
    ├── pages
    ├── sidebars.json
    ├── siteConfig.js
    └── static
```

### Running the website locally

1. Navigate to the `website` folder:
   ```
   cd website
   ```

2. Run the local web server: 
   ```
   yarn start
   ```

3. Navigate to the website: http://localhost:3000

### Publishing to GitHub Pages

The following properties were added to `website/siteConfig.js`:

```js
const siteConfig = {
    url: 'https://rikoe.github.io',
    baseUrl: '/FDC3/',
    projectName: 'FDC3',
    organizationName: 'rikoe'
}
```

To publish the website, follow this steps:

1. Navigate to the `website` folder:
   ```
   cd website
   ```

2. Publish: 
   ```
    GIT_USER=<GIT_USER> USE_SSH=true yarn run publish-gh-pages
   ```

This will publish to the `gh-pages` branch of the repository, which will automatically be hosted on GitHub Pages.

> For full documentation about publishing Docusaurus websites, see [Publishing your site](https://docusaurus.io/docs/en/publishing).

> For more information about GitHub Pages, see [GitHub's FAQ](https://help.github.com/articles/user-organization-and-project-pages/).