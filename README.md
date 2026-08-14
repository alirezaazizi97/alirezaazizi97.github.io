# Alireza Azizi — Academic Website

This is a deliberately simple academic website for GitHub Pages.

You only need two files for the website itself:

- `index.html` — the content of the page
- `styles.css` — the appearance of the page

No JavaScript, package manager, framework, server, or build step is required.

---

## 1. Put the files on GitHub

Your GitHub username is currently:

`alirezaazizi97`

For the default GitHub Pages address, the repository should therefore be named exactly:

`alirezaazizi97.github.io`

Upload `index.html` and `styles.css` to the **top level** of that repository.

The structure should look like:

```text
alirezaazizi97.github.io/
├── index.html
├── styles.css
└── README.md
```

Then your page will be available at:

`https://alirezaazizi97.github.io/`

It may take a few minutes after your first upload for GitHub Pages to publish.

---

## 2. The most important idea

Think of HTML as the **content and structure** of the page.

For example:

```html
<h1>Alireza Azizi</h1>
<p>This is a paragraph.</p>
```

CSS controls **what that content looks like**.

For example:

```css
h1 {
  font-size: 50px;
}
```

You can therefore make almost all routine updates by editing `index.html`
without touching `styles.css`.

---

## 3. Useful HTML tags

### Heading

```html
<h1>Alireza Azizi</h1>
```

`h1` is the main heading.

Smaller headings use:

```html
<h2>Research</h2>
<h3>Subsection</h3>
```

### Paragraph

```html
<p>This is a paragraph.</p>
```

### Link

```html
<a href="https://example.com">Click here</a>
```

The part inside `href="..."` is the destination.
The text between `>` and `</a>` is what the visitor sees.

### Bold

```html
<strong>Alireza Azizi</strong>
```

### Comment

```html
<!-- This is a comment. Visitors do not see it. -->
```

The template contains many comments to tell you what each section does.

---

## 4. Changing your bio

Open `index.html`.

Find:

```html
<section id="about" class="section">
```

Then edit the paragraphs below it.

For example:

```html
<p>
  I am a PhD student at ...
</p>
```

---

## 5. Changing research interests

Find this part:

```html
<div class="tag-list">
```

Each research interest has this form:

```html
<span class="tag">Differential Privacy</span>
```

To add a new one, copy the line:

```html
<span class="tag">New Research Topic</span>
```

To remove one, delete its line.

---

## 6. Adding a publication

Inside the `publications` section, one paper looks like:

```html
<article class="publication">
  <p class="pub-title">
    My Paper Title
  </p>

  <p class="pub-authors">
    <strong>Alireza Azizi</strong>, Coauthor Name
  </p>

  <p class="pub-venue">
    Conference Name, 2026
  </p>

  <p class="pub-links">
    <a href="https://...">Paper</a>
    <a href="https://...">arXiv</a>
  </p>
</article>
```

Copy that entire block and edit the contents for each new paper.

The `<strong>...</strong>` around your name makes your name bold.

---

## 7. Adding your CV

Put your PDF in the same repository, for example:

```text
cv.pdf
```

Then change:

```html
<a class="text-link" href="#">CV</a>
```

to:

```html
<a class="text-link" href="cv.pdf">CV</a>
```

Clicking **CV** will then open the PDF.

---

## 8. Adding your Google Scholar page

Find:

```html
<a class="text-link" href="#">Google Scholar</a>
```

Replace `#` with your Scholar URL:

```html
<a class="text-link" href="YOUR_GOOGLE_SCHOLAR_URL">Google Scholar</a>
```

---

## 9. Adding your email

Find:

```html
<a href="mailto:YOUR_EMAIL@example.com">YOUR_EMAIL@example.com</a>
```

Replace both appearances with your actual email.

Example:

```html
<a href="mailto:name@university.edu">name@university.edu</a>
```

The `mailto:` part makes the visitor's email app open when they click it.

---

## 10. Changing colors

You only need to edit the first few lines of `styles.css`.

For example:

```css
:root {
  --background: #ffffff;
  --text: #202124;
  --muted: #62676f;
  --border: #e5e7eb;
  --soft-background: #f7f8fa;
  --accent: #2457a7;
}
```

The most useful one is:

```css
--accent: #2457a7;
```

That controls the link/accent color.

---

## 11. Editing directly on GitHub

For a small change, you do not need Git or the command line.

1. Open your repository on GitHub.
2. Click `index.html`.
3. Click the pencil icon (**Edit this file**).
4. Make your changes.
5. Click **Commit changes**.
6. Wait a minute or two.
7. Refresh your website.

That is enough for normal updates.

---

## 12. Adding a photo later

Create a folder called:

```text
images
```

and upload a photo such as:

```text
images/profile.jpg
```

You can then add it to HTML with:

```html
<img src="images/profile.jpg" alt="Alireza Azizi">
```

The current template intentionally does not require a photo.

---

## 13. A few rules that prevent most mistakes

- Keep filenames lowercase when possible.
- Do not rename `index.html`.
- Keep `index.html` and `styles.css` in the same folder.
- HTML tags generally come in pairs:
  `<p> ... </p>`, `<a> ... </a>`, etc.
- Quotes around URLs are important.
- If the website suddenly looks broken, check the last thing you edited.
- GitHub keeps the history, so you can always restore an older version.

---

## 14. What you normally edit

For regular academic maintenance, you will mostly make only these changes:

1. Add a new paper.
2. Update your bio.
3. Update research interests.
4. Change your CV.
5. Add news or a new position.
6. Update links.

All of these can be done in `index.html`.

You can leave `styles.css` alone indefinitely if you like the current appearance.
