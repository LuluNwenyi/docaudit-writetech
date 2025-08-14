# Audit of Docusaurus Site

## Overview
This project intends to perform a simple audit of the Docusaurus site provided for the WriteTech Hub Accelerator Program.

### Goals
- Clone this repository.
- Review the folder and file structure.
- Submit your audit as a Markdown file named `audit.md` in the root of the repo.

---
# Project Summary
This repo features a stock Docusaurus template, which is designed to be easy to interpret, so that you can use it for your documentation site. 

Concepts and folders are presented simply, which invites the user to learn more about how to use Docusaurus. 

The goal of this audit is to perform a quick review of the structure and provide improvement suggestions, which will help me when I build out my first Docusaurus project. 

## Audit Summary
Here are some major findings from this audit:
- This repo displays standard folders, such as: 
    - `blog/`
    - `docs/`
    - `src/`
    - `static/`
- This repo also has additional, less standard folders and files:
    - `pages/`
    - `tutorials/`
    - `overview.md`

### Overall Structure

| Path                  | Purpose                                             | Suggestions                                                                    |
|-----------------------|---------------------------------------------------------------|--------------------------------------------------------------------------------|
| `docs/`               | Main documentation content (versionable, sidebar-driven)      | Consider sub-structuring by product/area as it grows.                          |
| `blog/`               | Blog posts, updates, release notes, longform                  | Keep if publishing updates; otherwise remove to reduce clutter.                |
| `static/`             | Static assets served at site root (images, files)             | Add subfolders (`img/`, `downloads/`) for better organization.                  |
| `src/`                | Site source (theme, components, and `src/pages`)              | Continue using for custom React components and theming.                         |
| `pages/`              | **Non-standard** at repo root                                 | Move content to `src/pages/` or remove if unused.                               |
| `tutorials/`          | Tutorials separate from `docs/`                               | Merge into `docs/` under a “Tutorials” section unless separation is intentional. |
| `overview.md` (root)  | Single Markdown page at root                                   | Move into `docs/` as an index or landing page.                                  |
| `docusaurus.config.js`, `sidebars.js` | Site and sidebar configuration                             | Keep configs close to content architecture.                                     |
| `README.md`, `CONTRIBUTING.md`        | Repo docs and contribution guidelines                        | Keep as is; expand if contribution process grows.                               |

# Notes
In the sections below, I've detailed my observations about this repo. I've separated these into the following sections:
- Organization Notes
- Inconsistencies

## Organization Notes
Here are some quick observations I made about the organization of this repo:

### Docs vs. Blogs vs. Pages

There is a clear separation between `docs`, `blogs`, and `pages` within this repo. 

However, since `pages/` is at the top-level, it makes the pages within the `src` directory seem redundant. This could pose future issues, such as being ignored by the build. 

I recommend consolidating the top-level `pages/` and the `pages` within the `src` folder.

### Tutorials as a Separate Top-Level

Tutorials are generally a subset of a company's `docs` directory. Having `tutorials` separate creates a bit of friction between `docs` and `tutorials`. 

If there are distinct owners or a publishing method that requires it, this may make sense, but otherwise, I recommend making `tutorials` a subset of `docs`.

### Root Content Files 
There are files in the root of this directory, such as `overview.md`. This impacts content discoverability and may make versioning or updating content difficult. 

I recommend placing these types of files in the `docs` folder. The only exception to this rule is `README.md`, which is useful within the GitHub repo.

### Future Processes
With the default configuration, features like linting and versioning are not yet enabled. Consider enabling these processes as you further develop this site.

---

## Inconsistencies 
Here are some inconsistencies I discovered during my audit:

### Non-Standard `pages/` Location
I recommend moving `pages/` to `src/pages`. If empty, I recommend removing `pages/` entirely and simply using the `src` directory.

### Integrate `tutorials`Into `docs/`'
I recommend moving `tutorials` into `docs/` and using the following structure:
```
docs/tutorials/
```
I also recommend splitting it into a sidebar category.

### Markdown File in Root
I recommend relocating `overview.md` into `docs/`:

```
docs/overview.md
```
Then, you can link to it from the sidebar, if needed.

### Information Architecture Not Defined
The default directory lacks a scalable information architecture (IA). 

Future versions of this site may need:
- Domains
- Roles
- Journeys

---

# Overall Recommendations
I've split my recommendations into the following categories:
- Quick Wins
- Structural Improvements
- Scalability Improvements

## Quick Wins
1. Remove or relocate `pages/` to `src/pages/`. This will reduce user confusion when navigating the website.
2. Move `overview.md` into `docs/`. You can add it to the sidebar so users can access it.
3. Place `tutorials/` into the `docs/` directory. You can add it in a `tutorials` category like this: `docs/tutorials`. 
4. Establish a clear naming convention. I recommend kebab-case for file names.

## Structural Improvements
1. Define a first-pass information architecture (IA) that reflects user intentions, such as Getting Started, Tutorials, and more.
2. Match the `sidebars.js` structure to my recommended IA structure in the Recommended Structure category below. This sidebar should have a maximum depth of 2 to keep it concise.
3. Introduce a content ownership rule for each folder to keep updates clean.

# Scalability Improvements
1. Enable link-checking or a continuous integration (CI) script. 
2. Adopt a doc linter (i.e. Vale) and establish a style guide (i.e., headings, acronyms, brand voice).
3. Prepare for Docusaurus doc versioning once v1 is tagged. 
4. Add search metadata (i.e., front-matter keywords) to all high-traffic pages.

---

# Recommended Structure
I've provided a sample IA structure, which can help in future editions of this site.

To better understand this structure, I've grouped it into the following categories:
- **Sidebar Groups:** Guides, Concepts, Reference, Tutorials
- **Blog:** Keep for announcements or release notes. If not used for those purposes, you can remove it to simplify your sitemap.
```csharp
docs/
  00-introduction/
    overview.md
    getting-started.md
  10-guides/              # task-based, stepwise
    installing.md
    configuring.md
    deploying.md
  20-concepts/            # explanations
    architecture.md
    key-terms.md
  30-reference/           # API/CLI/UI refs
    api/
      auth.md
      endpoints.md
  40-tutorials/           # longer, outcome-based
    build-a-hello-world.md
    integrate-with-x.md

```

# Recommended Conventions
I've provided a few general and stylistic considerations for you to follow below:

## General Conventions and Rules
I recommed creating rules and conventions for all of the pages within this Docusaurus site. You can do this by setting up a `YAML` file, or front-matter template. 

I've provided an example below of a front-matter template for an `installation` page. You can apply this concept to a single high-traffic page:

```yaml
id: installing             # Unique identifier for the page
title: Install the Toolkit # Title displayed at top of page
description: How to install and verify your setup.  # Used for SEO and search results
sidebar_position: 10       # Controls the order in the sidebar
tags: [install, setup]     # Helps with search and categorization

```
# Stylistic Considerations
I recommend using: 
- Sentence-case headings.
- Active voice.
- Present tense.
- One H1 per page.
- Images in static/img/`your image`.

# Checklist for Future Updates
- Use the provided IA structure for directory.
- Filenames in kebab-case.
- Front-matter completed for each new page.
- Add new pages to `sidebars.js`.
- Screenshots and assets should be placed in `static/`directory. 
- Site should build locally without errors before pushing to GitHub.
- Content should be signed off and reviewed by content owner (i.e., add them as a reviewer on your GitHub PR).

# What to Remove
- `blog/` should be removed if you do not plan on making updates, release notes, or announcements.
- `pages/` (at the top level) should be moved to `src/pages`.

---


# Conclusion
`README.md` states that this directory is a default Docusaurus configuration. 

Thus, for my suggestions, I have focused on setting up this project for clarity and scalability. I believe that a good documentation site is both maintainable and navigable. 

I hope that my notes and suggestions help this site grow into a complete future project.

---