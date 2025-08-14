# Documentation Audit Table

**Project Name:** docaudit-writetech
**Audit Date:**  August 13, 2025
**Auditor:**  Christine Belzie

---

## Structure & Organization

| Item                               | Status (✔/✖) | Notes                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
|------------------------------------|--------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `docs/` folder present             | ✅            | Contains separate folders for the site's "Getting Started", "Reference", and "Guides" sections.<br>Each folder has files for each topic.<br>For example, the `getting-started` folder has a `install.md` file (where the installation instructions are going to be written) while the `guides` folder has a `intro.md` file (where instructions on how to use the project are going to be written).                                                                                                             |
| `blog/` folder present             | ✅            | Contains a `welcome-2021-08-26` folder that has an image of a Docusaurus plushie as well as a  `index.md` file that has a blog post about Docusaurus. There's also files for other blog posts and a `authors.yml` and `tags.yml` files that contain blog post information. It would best for the plushie image to be in the `img` subfolder where the `assets` folder is. Also, turn the `2021-08-26-welcome` folder into to regular `welcome` folder, and make the `index.md` file the main page for the blog. |
| `pages/` folder present            | ✅            | Contains a `custom-page.md` file. It would be best to link that file from the main navigation.                                                                                                                                                                                                                                                                                                                                                                                                                  |
| `tutorials/` folder present        | ✅            | Meant to be for advanced users.  May need to be moved into the `docs` folder for easier navigation.                                                                                                                                                                                                                                                                                                                                                                                                             |
| `static/` folder present           | ✅            | Contains a `assets` folder that has an image that doesn't work. It would be best to remove it.  Also, there's a `img` subfolder.                                                                                                                                                                                                                                                                                                                                                                                |
| `overview.md` present and accurate | ❌            | Needs to be moved to the docs folder                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| `README.md` up-to-date             | ❌            | May need revising as it has too many Markdown errors                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| `CONTRIBUTING.md`                  | ✅            | Placed on the repository's root.  Makes it easier to find.                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| `sidebars.js` configured           | ✅            | Defines the sidebar navigation for your Docusaurus site, organizing documentation pages into sections and controlling their order and grouping.                                                                                                                                                                                                                                                                                                                                                                 |
| `docusaurus.config.js` configured  | ✅            | Sets up the main settings for the Docusaurus site, including its title, URL, navigation, theme, and plugins. It controls the site's structure and appearance.                                                                                                                                                                                                                                                                                                                                                   |
| Naming conventions consistent      | ✅            | File and folder names are descriptive and follow standard naming conventions such as `camelCase`, `snake_case`, or `kebab-case` with the file extension.                                                                                                                                                                                                                                                                                                                                                        |
| `package.json`                     | ✅            | Manages dependency and project metadata.                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| `package-lock.json`                | ✅            | Contains the dependencies and their versions.                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| `.gitignore`                       | ✅            | For files and directories users don't want to be seen in their GitHub repository.                                                                                                                                                                                                                                                                                                                                                                                                                               |

---

## Content Quality

| Item                           | Status (✔/✖) | Notes                                                                                                                                                                             |
|--------------------------------|--------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Covers all features            | ✅            | N/A                                                                                                                                                                               |
| Clear & concise language       | ✅            | N/A                                                                                                                                                                               |
| Consistent formatting/style    | ❌            | Frontmatter is missing in a lot of the files. For example, the [`install.md` file](/docs/getting-started/install.md) could use terms like `title:`, `description:`, and `image:`. |
| No broken links/images         | ✅            | N/A                                                                                                                                                                               |
| Updated for current version    | N/A          | N/A                                                                                                                                                                               |
| Examples/code snippets present | N/A          | N/A                                                                                                                                                                               |
| Tutorials consistent           | N/A          | N/A                                                                                                                                                                               |

---

## Accessibility & Usability

| Item                 | Status (✔/✖) | Notes                                                                                                                               |
|----------------------|--------------|-------------------------------------------------------------------------------------------------------------------------------------|
| Search works         | ❌            | Missing search bar. Adding one to the `docusaurus.config.js` file will make it easier for users to find what they're looking for.   |
| Navigation logical   | ❌            | Missing a search bar. Adding one to the `docusaurus.config.js` file will make it easier for users to find what they're looking for. |
| Mobile-friendly      | N/A          | N/A                                                                                                                                 |
| Headings structured  | ❌            | Some headings are missing and others are not formatted correctly.                                                                   |
| Images have alt text | ✅            | Alt text is present in the files that reference them and they are formatted correctly.                                              |

---

## Summary

**Top Issues:**  

1. Missing search functionality and navigation improvements needed for better usability.
1. Inconsistent formatting and missing frontmatter in documentation files.

**Key Recommendations:**  

1. Add a search bar and improve navigation structure in the site configuration.
1. Standardize formatting and add frontmatter to all documentation files for clarity and consistency.

## Action Plan

### Top Issues

1. Missing search functionality and navigation improvements needed for better usability.
1. Inconsistent formatting and missing frontmatter in documentation files.

#### Key Recommendations

1. Add a search bar and improve navigation structure in the site configuration.
1. Standardize formatting and add frontmatter to all documentation files for clarity and consistency.

### Next Steps

- Restructure folders for better organization, such as moving `overview.md` to the `docs` folder and organizing images/assets into appropriate subfolders.
- Add frontmatter to all documentation files for consistency.
- Implement a search bar and improve navigation in `docusaurus.config.js`.
