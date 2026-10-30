# Exercise 01 · Semantic profile page

**Goal:** Rebuild your HTML muscle memory by marking up a one-page professional profile with the *right* elements, not just `<div>`s.

## The task

Build a single page about yourself (real or placeholder content) in `index.html`, with light styling in `style.css`. It should include:

1. **Header:** your name as the page's only `<h1>`, and a `<nav>` with links that jump to each section below (`href="#about"`, etc.)
2. **About:** a `<section>` with a short bio and a profile image (a placeholder like `https://placehold.co/200` is fine)
3. **Skills:** a `<section>` with two lists: marketing skills and technical skills
4. **Featured work:** a `<section>` with at least two `<article>` elements, each with a heading, a short description, and a link
5. **Contact:** a `<form>` with name, email, a dropdown ("What's this about?"), a message `<textarea>`, and a submit button. No backend needed.
6. **Footer:** a `<footer>` with the year and a link to your GitHub

## Acceptance criteria

- [ ] Uses `<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<footer>` correctly
- [ ] Exactly one `<h1>`; headings go in order (no jumping from `h2` to `h4`)
- [ ] Every `<img>` has meaningful `alt` text
- [ ] Every form input has a `<label>` linked by `for`/`id`
- [ ] Email input uses `type="email"`; required fields use `required`
- [ ] Passes the [W3C validator](https://validator.w3.org/#validate_by_input) with no errors
- [ ] `style.css` sets fonts, colors, and spacing using at least 3 CSS custom properties (`--color-primary`, etc.)
- [ ] Page is readable at phone width (375px) with no horizontal scrolling

## Stretch goals

- Make the nav horizontal with Flexbox
- Add `:hover` and `:focus-visible` styles to links and buttons
- Run Lighthouse (Chrome DevTools → Lighthouse) and get Accessibility ≥ 95

## When you're done

1. Write `NOTES.md` here: two or three sentences on what was tricky and what you looked up.
2. Add a row to the progress log in the root `README.md`.
3. Commit and push, then ask Claude for a code review.

## Hints

<details>
<summary>Section vs. article?</summary>

An `<article>` makes sense on its own (you could syndicate it, like a blog post or project card). A `<section>` is a themed group of content that usually has a heading.
</details>

<details>
<summary>How do in-page nav links work?</summary>

Give the target an `id` (`<section id="about">`), then link to it with `<a href="#about">`. Add `html { scroll-behavior: smooth; }` for a nice touch.
</details>
