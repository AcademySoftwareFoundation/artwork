# Artwork Repository Template

This template repo is designed for a project to showcase logos easily in multiple formats. Generally speaking, a given project will prepare artwork in 2 formats (PNG & SVG) and at least 3 versions (color/black/white).

# How to use this template

After creating a new repository based on this template, there are generally three things you will need to do.

## Setup the \_config.yml file

The [\_config.yml](\_config.yml) file contains the base settings for the artwork repo, including naming, color schemes, default logos, and more. The file is well commented with the different options available.

## Create folders for each logo set

Next you will create folders for each logo set. You can either create the folders in a flat structure in the root directory of the repository, or have a nested structure to group like logo sets together ( for example, projects and other logos ).

In each folder, the key file to include is the `README.md` file. This file defines the layout for the logo set in the page, either using the default logo layout or by providing HTML and Markdown for a custom layout. Front matter options are as below:

```markdown
---
project_name: PROJECTNAME
description: __page description that will show in search results__
level: __grouping level for the main logo listing; must match the config setting category__
featured_image: __relative path to the feature image to use on the main logo listing__
layout: project ( default option, but can leave blank to put your own HTML in here )
---
```

## Add the images

The directory structure under the folder should look like...

logosetname
+--format1
  |--color1
    |--logosetname-format1-color1.svg
    |--logosetname-format1-color1.png
  |--color2
    |--logosetname-format1-color2.svg
    |--logosetname-format1-color2.png
+--format2
  |--color1
    |--logosetname-format2-color1.svg
    |--logosetname-format2-color1.png
  |--color2
    |--logosetname-format2-color2.svg
    |--logosetname-format2-color2.png

