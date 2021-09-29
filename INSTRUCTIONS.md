# How to add new project artwork

`<project full name>` is the display name for the project ( e.g. 'OpenEXR' )

`<project name>` is the name of the project in the filesystem ( e.g. 'openexr' )

1. Add a new directory under `projects` with the artwork. Artwork directory structure should map as follows...

```
<project name>
  - horizontal
    - color
      <project name>-horizontal-color.svg
      <project name>-horizontal-color.svg
    - white
      <project name>-horizontal-white.svg
      <project name>-horizontal-white.svg
    - black
      <project name>-horizontal-black.svg
      <project name>-horizontal-black.svg
  - stacked
    - color
      <project name>-stacked-color.svg
      <project name>-stacked-color.svg
    - white
      <project name>-stacked-white.svg
      <project name>-stacked-white.svg
    - black
      <project name>-stacked-black.svg
      <project name>-stacked-black.svg
  - icon
    - color
      <project name>-icon-color.svg
      <project name>-icon-color.svg
    - white
      <project name>-icon-white.svg
      <project name>-icon-white.svg
    - black
      <project name>-icon-black.svg
      <project name>-icon-black.svg
```
        
If you are using the GitHub web client, the easiest thing to do is create the folder structure on your local machine, and then go to the `projects` directory and follow the instructions for [uploading a folder/file to the repository](https://docs.github.com/en/repositories/working-with-files/managing-files/adding-a-file-to-a-repository)

2. Create `README.md` under `<project name>` directory. Contents should match this typically...

```markdown
---
description: Artwork for the <project full name> project
title: <project full name> 
level: <project level: match string on home page> 
featured_image: <relative path to the image to show on the home page> 
layout: logos
---
```
