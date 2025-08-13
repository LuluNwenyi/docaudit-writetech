# Audit report of the Docusaurus repo

### Pros of the site
- The use of the color green is appealing to the eyes
- There are custom pages i.e. `Tutorial`and `Blog` which allow the reader to choose what to view.
- In the `Tutorial intro` under `Tutorial` custom page, there is a hierarchy of information which enables the reader to know what to start with and proceed.
- The dark-mode feature adds a nice touch to the static site.

### Cons of the site
- There's a mismatch between the subtitle of ths site _Dinosaurs are cool_ and the content of the site.
- The title _My Site_ does not explain what the site is about. The reader is left guessing from the beginning.
- The `blog` custom page appears cluttered. Having the profile picture of the author, name, job title and all their socials in one element makes the blog appear busy and the reader is likely to experience information overload.
- There's the use of **bold** in areas where a link would be helpful

### Here's what can be improved
- Have a better title for your site. This gives the reader an idea of what to expect. 
- Punctuation and grammar. While there is a visible hierarchy of information in `Tutorial intro` under the `Tutorial` custom page, there is an improper use of punctuation. For example:

This:
```md
## Getting Started
Get started by creating a new site.

Or try Docusaurus immediately with docusaurus.new.
```

Rewritten as:
```md
## Getting Started
Get started by creating a new site or try Docusaurus immediately with [docusaurus.new](https://docusaurus.io/docs/playground).
```

- Add the necessary web links where needed. For example:
1. This:
```md
## Getting Started
Get started by **creating a new site**.
```
Could be re-written as:
```md
## Getting Started
Get started by [creating a new site](https://add-link-to-create-new-site)
```
2. This:
```md
### Generate a new site
Generate a new Docusaurus site using the **classic template**.
```

Could be re-written as:
```md
### Generate a new site
Generate a new Docusaurus site using the [classic template](https://link-to-the-classic-template)

### Conclusion
Overall, the site is visually appealing and covers the basics but there is a lot of room for improvement to make it much clearer and more intuitive to the reader.