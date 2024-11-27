# timekeepersmc

This is a hugo-powered static content site for the Timekeepers MC organization that can be viewed at [https://www.timekeepersmc.com](https://www.timekeepersmc.com)

# Editing

## Requirements

* hugo
* git

## Initialization

Once cloned, you need to run a `git submodule --init --recursive` to download the `hugo-hero-theme` into the `themes/hugo-hero-theme` or else the preview site will be blank as there is no theme for hugo to work with.

## Previewing Changes

You can run `hugo server` and access the local server to preview changes to the site. This will generally be hosted at [http://localhost:1313](http://localhost:1313)

## Static Content (Images and PDFs)

Static content such as images can be placed in the `static` directory and be referenced based on its subpath in the static directory. Thus, for a file called `ccse24-flyer-1.png` that is found at `static/tmc/ccse24-flyer-1.png`, you would refer to the file as `tmc/ccse24-flyer-1.png`.

For example, the following header of a page would refer to the `ccse24-flyer-1.png`:
```
---
title: 'Coyote Creek Sprint Enduro 2023'
date: 2024-11-27T09:00:00-07:00
draft: false
weight: 5
heroHeading: 'Coyote Creek Sprint Enduro 2024'
heroSubHeading: 'presented by The Timekeepers'
thumbnail: 'tmc/ccse24-flyer-1.png'
images: []
---
```

## Structure

The primary content (for the pages) of the site is in the `content` directory, and is based on the name of a `folder`.
