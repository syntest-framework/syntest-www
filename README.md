# Website for the SynTest Framework

This repo contains the sources for the SynTest Framework website.
The website is built on top of the popular open-source static site generator [Hugo](https://gohugo.io/) and makes use of the [Wowchemy](https://wowchemy.com/) theme.
The [Netlify](https://gohugo.io/) service is used to host the website.

## Adding material

Material can be added by anyone in any section.
For adding material, check [this documentation](https://wowchemy.com/docs/).

**Note:** Do not directly push your changes to the main branch. Instead, send a Pull Request (PR).

### Adding team members

Steps:

1. Run `hugo new --kind authors authors/<firstname-lastname>`
2. Update your information in **content/authors/<firstname-lastname>/index.md**
3. Replace **avatar.{jpg,jpeg,png,webp}** with your photo

## Build and preview locally

When making changes to the website, it is useful to build and preview the website locally before committing the changes to the repository.
Before you can build the website, you first need to install the following dependencies:

1. Install Hugo using [this documentation](https://gohugo.io/getting-started/installing/).
2. Install NPM using [this documentation](https://docs.npmjs.com/downloading-and-installing-node-js-and-npm)
3. Install the development dependencies: `npm install`

To preview the website:

1. Run `view.sh`

When an error occurs during building, try deleting the local Hugo cache:

- MacOS/Linux: `sudo rm -rf $TMPDIR/hugo_cache/`

## Deploy website

The website is automatically deployed whenever a new commit is merged into the main branch.
To see a preview of the changes in a PR, press the details link in the deploy status check.
