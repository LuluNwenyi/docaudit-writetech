# **The audit document**
This document contains an audit of the **docaudit-writetech** repository.

## **The main folders**
| Folder Name | Purpose |
| --- | --- |
| Blog | This folder contains blog posts |
| Doc| This contains the *Getting Started* and *Guides* files |
| Pages| This contains one custom page |
| src | This contains page features and CSS files
| static | This contains assets such as images |
| tutorials | This contains a README file |

## **The documentation organization**
Here are the details observed regarding the organisation of files and folders in the repository:
* Certain folders have unclear names, such as *static*
* Certain folders have similar sub-folders, for example, the docs folder has *getting started* and *guides*. Also,
* The arrangement of files wasn't uniform, for example, the *2021-08-26-welcome* folder under *blog* contains an image which should have been under *img* under *static* folder.
* There is no clear distinction between *tutorials* and *guides* under *docs*
* The *pages* under *src* seems redundant.
* There is no clear distinction between *blogs* and *pages*.

## **Suggestions for clarity**
Here are suggestions that can help improve the structure of the files and folders in the repository:
* The *static* folder can be renamed to *assets* for easy identification.
* The contents of subfolder *2021-08-26-welcome* should be moved to *assets* or *img* sunfolder.
* The files under the *blog* folder should be renamed for easier identification. Such as *2019-05-28-how-to-write-a-blog.md* instead of *2019-05-28-first-blog-post.md*.
* Redundant files and folders should be removed, such as the *pages* folder.
* 
* 
