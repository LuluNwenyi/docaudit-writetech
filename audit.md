# Documentation Repo Audit — Beginner View
**Repo audited** - `LuluNwenyi/docaudit-writetech`  
**Date audited** - August 13, 2025  
**Auditor** - Tochukwu Onyeama 

#### 1. Folder Structure and First-Thoughts Impressions
At first glance:
- **`docs/`**: This seems like it contains the main guides or instructions.
- **`blog/`**: This feels like a space for article-style updates. I’m guessing it might be for project news or tips
- **`pages/`**: Not entirely sure, but it sounds like custom pages, maybe the homepage or an about page? 
**`src/`**: From the looks of it, this is where the codes lives. I’m not familiar with it, so I skipped it 😬
**`static/`**: I know this is where images used in the documents are stored
**`tutorials/`**: This one confused me. Isn’t that the same as docs? Why is it separate?
**`overview.md`**: This seems like it should be in the docs section. I'm not entirely sure what it is for, seems like an introduction file
**Config files**: `docusaurus.config.js` and `sidebars.js` were intimidating at first. I can tell they control settings, but without comments or instructions, it’s hard to understand and it seems it should be inside the **`src`** file.



#### 2. Observations on Documentation Organization
The connections between folders aren’t obvious. For example, I don’t immediately know how `overview.md` links to the site or if `tutorials/` will show up in the sidebar.

I also noticed there’s no quick “map” that explains how all the folders fit together. I can guess from the names, but I might place files in the wrong spot if I were adding content as a non-programmer.

#### 3. Suggestions for Improvement (from a Beginner’s Perspective)
- Add short README files inside each folder to explain what belongs there.
- Merge or clarify `overview.md` so there’s just one clear starting point.
- In `docs/`, create a main welcome page that explains the structure.
- Add basic comments to config files saying what they control.
- Provide a simple “Getting Started” section in `CONTRIBUTING.md` for non-coders.

### Summary
The folder names give clues, but a little more explanation in READMEs and comments would make the repo much more beginner-friendly and easier to contribute to.