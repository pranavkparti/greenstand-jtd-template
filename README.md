# JTD template for Greenstand

This repo is intended to be used as a template for individual Greenstand project repositories. It sets up Jekyll with [Just The Docs](https://github.com/just-the-docs/just-the-docs) which can be used with Github Pages to display the project documentation.

The project documentation is assumed to be in the directory `docs/`. It is from where the Github Actions workflow builds the site.

## Usage

- Clone or download the template as `.zip`.
- Create a `.github/workflows` directory at the project root if your repo doesn't already have one. Copy the `pages.yml` file into this directory. GitHub Actions searches this directory for workflow files.
- Create a `docs/` directory at the project root (if it doesn't exist) and copy all remaining template files into this directory.

> Source: <https://github.com/just-the-docs/just-the-docs-template/blob/main/README.md#hosting-your-docs-from-an-existing-project-repo>


## Things to note

- It is recommended to have a parent page (typically named `index.md`) as the "entry point" to the documentation.
- The `docs/` directory may contain subdirectories like `api/`, `spec/`, etc., or other files which are not to be displayed and so should be added to the `exclude` attribute in `_config.yml`.