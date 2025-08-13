# Documentation Audit by Braimoh Victoria

## Folder Structure
The repo has main folders like:
- `docs` for the main documentation pages
- `blog` for posts or updates
- `pages` for static pages
- `src` for source files
- `static` for images or assets
- `tutorials` to serve as a learning material which should also be moved to the `docs` folder

Below the folders, there are a number of important files:
- `.gitignore` which lists files and folders Git should ignore.
- `CONTRIBUTING.md` explains how people can contribute to the project.
- `docusaurus.config.js` contains the main configuration for the Docusaurus site.
- `overview.md` should likely be a high-level description of the project which is supposed to be moved to the `docs` folder.
- `package-lock.json & package.json` manages the project’s dependencies.
- `README.md` file is a starting guide for anyone visiting the repo for the first time or without any clue on what the project is about.
- `sidebars.js` is meant to control the sidebar navigation in the documentation site.

## Observations on how the docs are organized
- The `docs` folder is split into small sections like getting-started and guides. The separation between docs, blog posts, and pages is clear, which makes it easy to understand and navigate. However, the files like `into.md` and `reference.md` are not properly placed and grouped.

- In addition, the files in the `docs` folder do not also contain sufficient information. The getting-started file has the installation guide which contains no installation instructions. The same goes for the reference and usage documents.

## Possible Improvements
1. Organise the `docs` folder properly. `Tutorials` and the `Overview.md` foldera should move into this folder.
2. The `intro.md` should be inside the getting-started file. It is basically an introduction and would be the first place a new reader would look at.
2. Add proper categories to the sidebar for easier navigation.
3. Update the README to explain:
   - What the project is about
   - How to run the docs locally
   - You can choose to move the current assessment questions to the bottom of the READMe after adding the overview of what the project is about or create a new file titled `Assessment`
4. Update the installation guide, the usage.md and the reference.md to include proper information.
5. Finally, add a short “Contributing to Docs” section to guide anyone who wants to help improve them.