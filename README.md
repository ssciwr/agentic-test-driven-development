# Course Slides Template

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

Template for a course repo that includes SSC-themed slides that are automatically built in CI as html and pdf.
Click the "Use this template" button the top right to create a new repo using this template, then enable github pages with Source "GitHub Actions".

## Slides

[![Course slides](https://ssciwr.github.io/course-slides-template/slides-thumb.png)](https://ssciwr.github.io/course-slides-template)

[Download as PDF](https://ssciwr.github.io/course-slides-template/slides.pdf)

## Marp

[Marp](https://marp.app/) slides are just markdown, with `---` to separate the slides, and some frontmatter at the top of the file, e.g.

```markdown
---
marp: true
theme: ssc
paginate: true
title: Course Title
description: SSC Compact Course
---
```

## SSC theme

There is an SSC theme provided in [slides/ssc.css](slides/ssc.css).
You can also add optional per-slide classes (apply with `<!-- _class: name -->`):
 - `title`: title slide (large heading, dark background, big combined logos top-right)
 - `subtitle`: subtitle slide (centered heading, dark background)
 - `hands-on`: adds a hands-on indicator to the top-left corner of the slide

## Local rendering

To render the slides locally:

```bash
npx @marp-team/marp-cli@latest -w slides
```

Then you can open slides/index.html in a browser and see the changes when you edit slides/index.md.