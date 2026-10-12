# Griffin Chipato - Profile & Mini-Portfolio

A semantic HTML5 profile and mini-portfolio website showcasing my background, skills, projects, and contact information.

## About the Project

This project was created as part of the Web Technologies (CIS2103) practical assignment. The website uses semantic HTML5 elements to create a clear and accessible one-page profile and portfolio.

The website includes:

* Home/Profile section
* About Me section
* Skills section
* Contact section
* Contact form with HTML5 validation
* Footer

## Technologies Used

* HTML5
* CSS3
* Git
* GitHub
* AI-assisted content generation

## Semantic HTML5

The website uses semantic HTML5 elements including:

* `<header>` – contains my name and tagline.
* `<nav>` – contains links for navigating between page sections.
* `<main>` – contains the main content of the webpage.
* `<section>` – separates the different areas of the portfolio.
* `<article>` – used for individual portfolio/project content where appropriate.
* `<footer>` – contains the copyright information.

## Contact Form

The Contact Me form uses different HTML5 input types and native validation.

The form includes:

* Name – text input
* Email – email input
* Phone – telephone input
* Message – textarea
* Required fields
* Appropriate labels connected to their inputs

## AI-Assisted Content

AI was used to help develop the initial About Me content and tagline. The generated content was reviewed and edited so that the final version better represents my own background, interests, and writing style.

The complete AI prompt, raw AI output, edited version, and reflection are available in:

**`PROMPT_LOG.md`**

## Accessibility Issue and Fix

During peer review, an accessibility issue was identified with the website.

**Issue:** Some form fields did not have clearly associated labels, which could make it difficult for users, including users of assistive technologies, to understand what information should be entered.

**Fix:** I added `<label>` elements and connected each label to its corresponding input using matching `for` and `id` attributes.

For example:

```html
<label for="email">Email:</label>
<input type="email" id="email" name="email" required>
```

This makes the form easier to understand and improves accessibility.

## Version Control

Git was used throughout the development of the project. The project was developed using multiple meaningful commits rather than submitting everything in a single commit.

Examples of development stages include:

* Created initial HTML structure
* Added semantic sections and navigation
* Added contact form and validation
* Improved accessibility and page presentation

## Author

**Griffin Chipato**

Computer Information Systems Student

## Repository

This project is hosted on GitHub as part of the Web Technologies coursework.

# Griffin Chipato - Portfolio

Profile / mini-portfolio page for Web Technologies (CIS2103), Africa University.

## Responsive Notes

**Breakpoints tested** (browser device toolbar): mobile (~375px), tablet (~768px) and desktop (~1280px). There is no horizontal scrolling, overlapping text or broken navigation at any of them.

**Flexbox vs. Grid**
- **Flexbox** is used for one-row or one-column layouts: the header and nav, the Contact form fields, and the footer.
- **Grid** is used for the Skills section, because the cards sit in rows and columns that reflow with `repeat()`, `fr`, `minmax()` and `gap`.

**Tailwind vs. my own CSS**
- **Tailwind utilities:** the header/nav and the Contact form, including the responsive variants `md:` and `sm:`.
- **My own CSS (`styles.css`):** the base styles, typography, About and Skills sections, the footer, and the custom `min-width` media queries (768px and 1280px).

The CSS is written mobile-first and layered up to larger screens with `min-width` media queries.