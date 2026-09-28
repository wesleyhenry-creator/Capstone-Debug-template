# My Personal Portfolio Website

## Overview

This project is a responsive personal portfolio website built with HTML and CSS. It introduces the developer, highlights web development skills, presents sample projects, and provides a contact form for potential collaborators or employers. The website is organized into four pages: Home, About Me, Projects, and Contact.

## Issues Found

The starter code contained several errors, inconsistencies, and omissions:

* Some pages did not initially include consistent main navigation, making it difficult to move between pages.
* Some image references did not match the image files available in the project.
* The starter markup used inconsistent indentation and formatting.
* Some pages were missing descriptive meta descriptions.
* Project content initially appeared in a single vertical layout instead of using a responsive multi-column layout on larger screens.
* Some form fields did not have sufficient HTML5 validation.
* The phone field required a correctly associated label.
* The contact form initially lacked a semantic `fieldset` and `legend` for the radio-button group.
* Some page sections used generic layout elements where more meaningful semantic elements could be used.
* The navigation needed correct `aria-current` usage so that only the active page was identified.
* The CSS contained an invalid `max-width` value that needed to be corrected.
* The site required improved keyboard-focus states for accessibility.
* Some images needed more descriptive alternative text.
* The project cards needed clearer semantic structure.
* The website required improved responsive behavior for smaller screens.

## Fixes Implemented

The current implementation includes descriptive page metadata, meaningful image alternative text, explicit image dimensions, structured headings, semantic HTML elements, and a responsive contact form.

The Home page now includes two semantic project cards using `<article>` elements. The Projects page contains three project cards, also using semantic `<article>` elements.

The contact form has been improved with:

* Associated labels for all form controls
* Text, email, telephone, select, radio, and textarea controls
* Required fields
* `minlength` and `maxlength` validation
* A telephone `pattern` attribute
* `autocomplete` attributes
* A semantic `fieldset` and `legend`
* A submit button

The stylesheet provides responsive layouts, navigation hover states, keyboard-focus states, styled project cards, table styling, form validation feedback, consistent spacing, and mobile-friendly layouts.

## HTML Structure and Semantics

Each page uses semantic HTML elements including `header`, `nav`, `main`, `section`, `article`, `figure`, `figcaption`, and `footer`.

The pages use a logical heading hierarchy with a page title followed by section and content headings.

The About Me page includes a captioned skills table containing:

* `<thead>`
* `<tbody>`
* `<th>`
* `<td>`
* Column scopes
* Three skill rows

The Projects page uses semantic `<article>` elements for each project and `<figure>` elements for project images and captions.

The Home page contains two project cards that provide a quick overview of selected work.

The Contact page uses a semantic `<form>` with associated labels, appropriate HTML5 input types, validation attributes, autocomplete hints, a radio-button fieldset, and a submit button.

## CSS Approach

The main stylesheet is located at:

`portfolio/css/styles.css`

The stylesheet begins with global box sizing and base typography before defining reusable styles for the header, navigation, main content, sections, hero area, project cards, tables, images, forms, links, and footer.

Class selectors such as `.hero`, `.intro`, `.work`, `.project`, `.projects-grid`, and `.footer` provide reusable styling.

Element selectors such as `body`, `nav`, `nav a`, `form input`, `table`, and `figure` keep repeated patterns consistent.

The Projects page uses `.projects-grid` to display three project cards in equal columns on larger screens. The Home page uses the `.work` section to display two featured project cards.

The responsive media query changes the Projects layout to one column below `600px` and also adapts navigation, spacing, typography, forms, and table padding for smaller screens.

Pseudo-classes including `:hover`, `:focus`, `:focus-visible`, `:valid`, `:invalid`, and `:nth-child()` provide interaction, accessibility, and form-state styling.

## Accessibility Improvements

The website includes several accessibility improvements:

* `lang="en"` on every HTML document
* Descriptive page titles
* Meta descriptions
* Navigation labels using `aria-label`
* `aria-current="page"` on the active navigation link
* Descriptive image `alt` text
* Figure captions where appropriate
* Table headers using `scope="col"`
* Explicit labels for form controls
* Semantic form controls
* Required-field validation
* Email and telephone validation
* `autocomplete` attributes
* Keyboard focus indicators
* Visible hover and focus states
* Semantic `fieldset` and `legend` for the contact-method radio buttons

These improvements make the website easier to navigate and understand for both keyboard users and users of assistive technologies.

## View Locally

Download the project ZIP file and extract it to your computer.

Alternatively, clone the repository and navigate to the project folder.

Open the `portfolio` folder in Visual Studio Code and launch `index.html` using the **Live Server** extension. You can then select **Open with Live Server** to preview the website in your browser.

The main page is:

`portfolio/index.html`

The other pages are:

* `portfolio/about.html`
* `portfolio/projects.html`
* `portfolio/contact.html`

The stylesheet is located at:

`portfolio/css/styles.css`

## Screenshots

### About Me Page

[About Me Screenshot](https://github.com/wesleyhenry-creator/Capstone-Debug-template/blob/c357f55d03af16cf7bf9eb7cc7770e173333e935/portfolio/screenshots/aboutme.png)

### Contact Page

[Contact Page Screenshot](https://github.com/wesleyhenry-creator/Capstone-Debug-template/blob/8dcb670e13dbbbafa7b44920ea59039d97bbd63e/portfolio/screenshots/contact.png)

### Home Page

[Home Page Screenshot](https://github.com/wesleyhenry-creator/Capstone-Debug-template/blob/8334d2ea1bef4a3096d5a3082d75d59a39e143a6/portfolio/screenshots/index.png)

### Web/Mobile View

[Responsive Website Screenshot](https://github.com/wesleyhenry-creator/Capstone-Debug-template/blob/dd4f5a16c6e40ca8c948a78ade840e944dadf6d0/portfolio/screenshots/completed-website.png)

### Projects Page

[Projects Page Screenshot](https://github.com/wesleyhenry-creator/Capstone-Debug-template/blob/8da7ca50819c441b99711aaecadd121fcdf0bb4a/portfolio/screenshots/before-project.png)

## Reflection

The most challenging part of the project was identifying the difference between visual problems, HTML structure problems, missing assets, and CSS issues.

I compared referenced image files with the available assets, reviewed the HTML structure of each page, and checked the CSS selectors against the classes and elements used throughout the website.

Adding semantic HTML elements improved the structure of the website, while explicit form labels, validation attributes, and keyboard-focus states improved accessibility.

Creating responsive CSS also helped ensure that the navigation, project cards, forms, tables, and other content remain usable on smaller screens.

The project also helped me understand the importance of validating HTML and CSS, maintaining consistent code formatting, using meaningful semantic elements, and testing a website at different screen sizes.

Overall, the debugging and improvement process resulted in a more structured, accessible, responsive, and user-friendly personal portfolio website.
