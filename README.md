# Example Single FDC3 Repository and Website

This repository demonstrates using [Docusaurus](https://docusaurus.io) to author and host the FDC3 website and documentation, based on markdown files.

## Plan

* Try out Docusaurus
* Host on GitHub Pages
* Attempt to apply styling and assets from https://fdc3.finos.org to this website
* Copy content from other FDC3 repositories into this single repository, to try and achieve a unified structure with an overview, that distinguishes clearly between specifications, examples and usage documentation
* Apply versioning
* Add documentation content

## Developer Information

The included example website was generated by following the [Docusaurus installation steps](https://docusaurus.io/docs/en/installation).

### Required tools

* NodeJS 8+ [[Install](https://nodejs.org/en/download/)]
* Yarn 1.5+ [[Install](https://yarnpkg.com/lang/en/docs/install/)]
* Docker [[Install](https://www.docker.com/get-started)]

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