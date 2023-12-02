---
title: "Space: Multifunction Screenshot Application based on QT"
draft: false
date: 2021-11-23
description: "The inspiration for this software comes from when organizing notes. I hope that taking screenshots from PPT or other materials can remove the background color and ensure the neatness of the notes."
language: 'C++/QT'
platform: 'Windows/MacOS'
link: 'https://github.com/InkosiZhong/Space'
tags:
  - Developments
---

> Access [Space product page](http://foldimension.tech/#/) for more interactive experience.
### Background Removal
Space can remove the background in the courseware (PPT etc.), making it easier to unify the style of notes.

![remove background](rmbg.png)

### Smart OCR
Space will automatically detect whether the text content belongs to the same paragraph, simplifying user operations as much as possible. When the content does not belong to the same paragraph, Space provides an efficient candidate window.

![smart ocr](ocr.png)

### LaTeX Formula Extraction
Formulas are another type of items that appear frequently in courseware. 
Space can quickly extract the LaTeX code corresponding to the formula for easy reproduction.

![latex extraction](latex.png)