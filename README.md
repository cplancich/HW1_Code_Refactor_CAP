# Code Refactor Challenge

## User Story

```
AS A marketing agency
I WANT a codebase that follows accessibility standards
SO THAT our own site is optimized for search engines
```

## Acceptance Criteria

```
GIVEN a webpage meets accessibility standards
WHEN I view the source code
THEN I find semantic HTML elements
WHEN I view the structure of the HTML elements
THEN I find that the elements follow a logical structure independent of styling and positioning
WHEN I view the image elements
THEN I find accessible alt attributes
WHEN I view the heading attributes
THEN they fall in sequential order
WHEN I view the title element
THEN I find a concise, descriptive title
```

## Changes Made

### Semantics

* Line 7, changed `<title>` from "webpage" to "Horiseon Social Solution Services" (found in footer)

* Line 11, changed `<div class="header">` tag to `<header class="header">`

* Line 13, changed `<div>` tag to `<nav>` tag, altered styling classes in style.css document on lines 27, 35, and 39 to apply to updated `<nav>` tag

* Line 27, added `alt` tag for background hero image

* Line 28, changed `<div>` tag to `<main>`

* Lines 29, 36, and 43; changed `<div>` tag to `<article>`

* Lines 30, 37, and 44; added `alt` tags to `<main><article>` images

* Line 51, changed `<div>` tag to `<aside>`

* Lines 52, 59, and 66; changed `<div>` tags to `<article>`

* Lines 54, 61, and 68; added `alt` tags to `<aside><article>` images

* Line 74, changed `<div>` tag to `<footer>`

* Lines 75 and 76; changed `<h2>` and `<p>` tags to `<h4>` and `<h5>` (per acceptance criteria, WHEN I view the heading attributes THEN they fall in sequential order)

### Other

* Consolidated redundant CSS classes
    * `.benefit-lead`, `.benefit-brand`, and `.benefit-cost` consolidated to `.benefit`, applied changes to html selectors
    *  `.online-reputation-management`, `.social-media-marketing`, and `.search-engine-optimization` classes consolidated to new `.article-bg` class, applied new class to other redundant occurances previously applied to elements within new `.article-bg`; updated html selectors with new `.article-bg` class


* Removed unnecessary id selectors from `.article-bg` class selected elements in index.html

## Deployed Application

Per the assignment, the deployed page looks exactly like the old one, but code has been updated to reflect clear semantics and consolidate redundant code. 

![Deployed Website](assets/images/Readme-preview.png)
