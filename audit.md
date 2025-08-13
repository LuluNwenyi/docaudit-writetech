# Repository Audit Documentation By Oluwaseitan Seyitan

## 1. Folder Structure
- **blog/** => Contains Markdown blog posts, and updates.
- **docs/** => Contains documentation content in their different topics.
- **pages/** => Contains the pages.
- **src/** => Contains the app source files
- **static/** => Contains static assets like images and fonts.
- **tutorials/** => This folder contains tutorials for advanced users.

**Files in Root Folder:**
- `README.md` => Introduction to the project.
- `overview.md` => Overview of the document.
- `CONTRIBUTING.md`.=> Should ive details on how people can contribute to the project.
- `docusaurus.config.js`=> Docusaurus comfiguration file.
- `sidebars.js` => To create an ordered group of docs, render a sidebar for each doc of that group, and provide next/previous navigation.

- `package.json` => Manages dependency and project metadata.
- `package-lock-json`=> ""
- `.gitignore` => For files and directories you don't want to be seen in your GitHub repository.
---



## 2. Observations on How Docs Are Organised
- Docs, blog, pages, src, and static are clearly separated into their own folders.
- `sidebars.js` helps create an ordered group of docs.
- The `install.md` file is empty. Thus, no installation uie for users.
- `tutorials/` is outside of the docs folder, which could confuse contributors.
- `overview.md` exists in the root folder, which shouldn't be.
- The docs are easy to navigate but files like `intro.md` and `reference.md` are not properly placed. As mentionedearlier,the `overview.md` file and the `tutorials/` folder are not properly placed.
- The `intro.md` file in the `docs/` folder is not place rightly.
---

## 3. Notes on Possible Improvements
1. The `tutorials/` folder should be merged into `docs/` for a better structure.The folder should be alongside the sub-folders in the `docs/` folder.
   
2. Move `overview.md` to the `docs/` folder for a better file structure. The file should be alongside the `reference.md` file in the `docs/` folder.
3. The `intro.md` file in the `docs/` folder should be in the `getting-started/` sub-folder that's in the `docs/` folder.
4. There should be a general readme file that explains each folder and it's application.
5. The `install.md` file should be filled with the installation instructions for users.
   

   


---
