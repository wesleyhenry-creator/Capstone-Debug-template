# My Personal Portfolio Website

## Overview

This project is a responsive personal portfolio website built with HTML and CSS. It introduces the developer, summarizes skills, presents sample projects, and provides a contact form for potential collaborators or employers. The site is organized into four pages: Home, About Me, Projects, and Contact.

## Issues Found

The starter code contained several errors and omissions:

- The About, Projects, and Contact pages did not include the main navigation, making the site difficult to explore.
- The third project referenced `images/project3.jpg`, but that asset was not available in the images folder.
- Starter markup used inconsistent indentation and lacked some page-level descriptions.
- Project sections initially appeared in one vertical column instead of displaying beside one another on larger screens.
- Missing navigation between pages.
- Placeholder-only fields are not enough for a usable contact form.

## Fixes Implemented

The current implementation adds descriptive metadata where needed, meaningful image alternative text, explicit image dimensions, structured headings, a labeled contact form, and responsive image sizing. The stylesheet also supplies visible hover and keyboard-focus states, mobile navigation behavior, validation feedback, consistent spacing, and reusable layout styles.

## HTML Structure and Semantics

Each page uses `header`, `nav` where provided, `main`, `section`, and `footer` landmarks. Headings follow a logical hierarchy, with one page title and nested section headings. The About page uses a captioned table with column scopes for skills. The Contact page uses a `form` with associated `label` elements, semantic input types, autocomplete hints, required fields, and a submit button. Images include descriptive `alt` text and dimensions.

## CSS Approach

`portfolio/css/styles.css` begins with global box sizing and base typography, then defines reusable selectors for the header, navigation, main content, sections, projects, tables, images, forms, links, and footer. Class selectors such as `.hero`, `.intro`, `.work`, `.project`, `.projects-grid`, and `.footer` provide page-specific styling, while element selectors such as `nav a`, `form input`, and `table` keep repeated patterns consistent. `.projects-grid` uses three equal responsive columns with consistent gaps; its media-query rule changes the layout to one column below `600px`. Pseudo-classes (`:hover`, `:focus`, `:focus-visible`, `:valid`, and `:invalid`) communicate interaction and form state. The media query also adapts navigation, spacing, typography, and table padding for smaller screens.

## Accessibility Improvements

The site includes the document language, viewport metadata, descriptive page titles, navigation labeling, current-page indication on the Home link, meaningful image alternatives, table headers with scopes, explicit form labels, required-field and email validation, autocomplete attributes, and high-visibility keyboard focus outlines.

## View Locally

Download the zip file and you can view it by "view in browser". Or clone the URL repository and cd into the path. Open index.html directly in a browser on  VS Code Live Server and select show preview or "Open with live server"

## Screenshots

https://github.com/wesleyhenry-creator/Capstone-Debug-template/blob/c357f55d03af16cf7bf9eb7cc7770e173333e935/portfolio/screenshots/aboutme.png

https://github.com/wesleyhenry-creator/Capstone-Debug-template/blob/8dcb670e13dbbbafa7b44920ea59039d97bbd63e/portfolio/screenshots/contact.png

https://github.com/wesleyhenry-creator/Capstone-Debug-template/blob/8334d2ea1bef4a3096d5a3082d75d59a39e143a6/portfolio/screenshots/index.png

## Reflection

The most challenging part was separating visual problems from path. I compared every referenced asset with the actual folders, checked the HTML structure around the broken footer, and reviewed the CSS selectors against the classes used in each page. Testing at a narrow viewport also exposed where the navigation and content needed responsive rules. Using semantic elements, explicit labels, and focus states resolved both usability and accessibility issues without adding JavaScript or unnecessary dependencies.
