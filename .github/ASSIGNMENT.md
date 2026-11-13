# 📄 Background Images

Use the CSS `background-image` property and its related properties to add, repeat,
position, and size images inside HTML elements.

## 🎯 Overview

In this coding exercise, you will add background images to a page that explains how
background images work. You will tile a pattern across the page, stretch a photo across
the header, and place small graphics exactly where you want them inside an element.

Background images are different from the HTML `<img>` element. An `<img>` is content: it
takes up its own space on the page and needs `alt` text. A CSS background image is
decoration: it sits **inside** an element's box, behind the content, and doesn't take up
any space of its own. Use `<img>` for images that carry meaning and CSS backgrounds for
images that are only there for looks.

The page itself is a reference sheet. As you work, read the content in `index.html` — it
describes the same properties you are practicing.

> [!IMPORTANT]
> **The companion video for this exercise is in Canvas**, on the assignment page. It walks
> you through every step, so watch it there instead of working from this file alone.

## 🧠 What You Will Learn

By completing this exercise, you will practice how to:

- Add an image to an element with `background-image: url();`
- Write file paths in `url()` so the browser can find your images
- Control tiling with `background-repeat` (`no-repeat`, `repeat-x`, `repeat-y`, `repeat`)
- Place an image with `background-position` using keywords, percentages, or pixels
- Scale an image with `background-size` (`cover`, `contain`, percentages, or pixels)
- Combine several background properties into the `background` shorthand
- Explain when to use a CSS background image instead of an HTML `<img>` element

## 🎬 Watch the Video in Canvas and Follow Along

The screencast video is on this assignment's page in **Canvas**, not in this repo. Watch it
and follow along in Visual Studio Code. Pause whenever you need time to finish a step — it
is normal to pause, rewind, and rewatch parts of a coding demonstration.

Make your changes as the video makes them. Save and refresh your browser often so you can
see what each property does.

> [!IMPORTANT]
> **A few steps in this repo are different from Canvas and the video.** Follow the video
> for the CSS, and follow this repo for getting your files and submitting:
>
> - **Getting the starter files:** don't download the ZIP from Canvas. Create your own repo
>   from this template and clone it in WebStorm, as described in the
>   [Getting Started guide](GETTING_STARTED.md).
> - **Branch:** do your work on a `develop` branch, not `main`. Before you commit, the
>   branch name at the top left of WebStorm should say `develop`, not `main`.
> - **Submitting:** don't zip your folder or upload a file. Publish your page to GitHub
>   Pages, open a pull request into `main`, and submit the **pull request URL** in Canvas,
>   as described in the [Submitting guide](SUBMITTING.md).

> [!IMPORTANT]
> Open the entire project **folder** in VS Code, not a single HTML file. Your CSS needs to
> find the image files, so keep every starter file together in the root folder.

## 📂 Starter Files

| File | Purpose |
| --- | --- |
| `index.html` | The page content. You shouldn't need to change it. |
| `styles.css` | Your stylesheet. Write your background rules in the section under the **Add background images** comment at the top. Leave the **No changes needed** section alone. |
| `reset.css` | Removes browser default styles so every page starts from the same blank slate. Don't edit it. |
| `tile.png` | A small, seamless pattern. Made to repeat across a large area. |
| `bkg_header.jpg` | A wide red graphic. Made to fill the page header. |
| `watermark.png` | A faint UC logo. Made to sit behind text without getting in the way. |
| `c-paw.png` | A small Bearcats paw logo. Made to be placed once, in a specific spot. |
| `positions.png` | A diagram of `background-position` values. It is already on the page as an `<img>` — it is content, not a background. |

`index.html` already links `reset.css` and then `styles.css`, in that order. Keep it that
way so your styles build on top of the reset.

Because `styles.css` and the images are in the same folder, the path inside `url()` is just
the file name, like `url(tile.png)`.

## ✅ Before You Submit

Check the following:

- [ ] `index.html` still links `reset.css` and `styles.css`, and your styles show up in the browser
- [ ] Your background rules are in the **Add background images** section of `styles.css`
- [ ] Every image file name in `url()` is spelled exactly right, including the extension
- [ ] Each background image from the video appears on the page
- [ ] A pattern repeats where it should, and images that should appear once use `no-repeat`
- [ ] At least one background image is placed with `background-position`
- [ ] At least one background image is scaled with `background-size`
- [ ] At least one rule uses the `background` shorthand
- [ ] Text is still easy to read on top of every background image
- [ ] You saved your files
- [ ] The page is live on GitHub Pages and the URL is in your pull request

## 🧮 Grading Rubric

| Criteria | Full credit | Points |
| --- | --- | --- |
| **Adding background images** | Each background image from the video is added with `background-image: url();` or the `background` shorthand. Every file path is correct, so every image loads. | 2 |
| **Repeating** | `background-repeat` is used correctly: patterns tile where they should, and single images use `no-repeat`. | 2 |
| **Positioning and sizing** | `background-position` places images where intended, and `background-size` scales them to fit their elements. | 2 |
| **Shorthand and readability** | At least one rule combines properties in the `background` shorthand. Text stays readable on top of every background, and the starter styles are intact. | 2 |
| **Publishing and submission** | The page is live on GitHub Pages. The pull request from `develop` into `main` is open, its template is filled in, and its URL is submitted in Canvas. | 2 |
| **Total** |  | **10** |

## 🛠️ Troubleshooting

If something is not working, check these common issues first:

- Did you save the file in VS Code?
- Is the image file name in `url()` spelled correctly, including `.png` or `.jpg`?
- Is the image in the same folder as `styles.css`? If not, the path in `url()` has to include the folder.
- Did you close the parentheses and end the line with a semicolon: `url(tile.png);`?
- Is the element big enough to show the image? A background image only fills the element's box — an empty or tiny element won't show much.
- Is a later rule overriding yours? A `background` shorthand resets every background property it doesn't list, including `background-color`.
- Did you commit **and** push your changes in WebStorm?

**Having problems with the video?**

- **Getting a warning about third-party cookies?** Try using Chrome. Safari's default
  security settings may prevent embedded Canvas videos from playing unless those settings
  are changed.
- **Getting an "Access Denied" error?** Refresh your browser. In many cases, the video
  will load correctly after the page reloads.

## 📚 Resources

- [MDN — `background-image`](https://developer.mozilla.org/en-US/docs/Web/CSS/background-image)
- [MDN — `background-repeat`](https://developer.mozilla.org/en-US/docs/Web/CSS/background-repeat)
- [MDN — `background-position`](https://developer.mozilla.org/en-US/docs/Web/CSS/background-position)
- [MDN — `background-size`](https://developer.mozilla.org/en-US/docs/Web/CSS/background-size)
- [MDN — `background` shorthand](https://developer.mozilla.org/en-US/docs/Web/CSS/background)
- [MDN — Backgrounds and borders](https://developer.mozilla.org/en-US/docs/Learn_web_development/Core/Styling_basics/Backgrounds_and_borders)
- [W3C CSS Validation Service](https://jigsaw.w3.org/css-validator/#validate_by_input) —
  paste your CSS in to catch typos and missing semicolons

---

The AI policy and submission instructions are in the [README](../README.md).
