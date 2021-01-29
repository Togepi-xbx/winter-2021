---
layout: post
title: Card patterns
categories: cpnt260
---

## Homework
1. Review
    - [Images in HTML](https://developer.mozilla.org/en-US/docs/Learn/HTML/Multimedia_and_embedding/Images_in_HTML)
2. `figure` element
    - Read: [The figure with optional caption element](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/figure)
    - Read: [Replaced elements](https://developer.mozilla.org/en-US/docs/Web/CSS/Replaced_element)
3. Cards
    - Read: [Card](https://developer.mozilla.org/en-US/docs/Web/CSS/Layout_cookbook/Card)
4. Preserving image aspect ratio
    - Reference: [`object-fit`](https://developer.mozilla.org/en-US/docs/Web/CSS/object-fit)
    - Read: [Cropping Images in CSS With object-fit](https://www.digitalocean.com/community/tutorials/css-cropping-images-object-fit)

---

## Morning reflection
### Housekeeping
1. Tooltime
    - VS Code: Split screen
2. Dailies feedback
    - Types of errors
        1. Syntax errors
            - validate
            - VS Code Extention: HTML Hint (v0.10)
        2. Logic errors
            - Inspect the element
            - Is the problem html or css?

---

## Tooltime: Evaluating VS Code extensions
 - HTMLHint vs HTMLLint vs another HTMLHint?

### Learning objectives
- Compare two things with VS Code split screen.
- Evaluate extension search results.
- Optional: install a VS Code extention.

### Activity: Extension window shopping
In groups of 3 or 4, search, share and/or install useful VS Code extensions.

### Favourites
- 

## Lecture/Live code
### Learning Objectives
- Define replaced elements.
- Undertand the cause of broken aspect ratio on images (hint: it's probably `height`).
- Learn the wonders of `cover` and `contain`.

### Terms
Aspect ratio
: `width` divided by `height` (usually).

`cover`
: Crop the longest axis (main axis) until the cross-axis fills the container.

`contain`
: Fit the longest axis (main axis) to the container. Extra space is transparent background?

### Materials
- [Norville's sweet sandbox](https://nozky.github.io/playground/).

### Key Takeaways
- Defining both a `width` and `height` is often bad for `img` and `background-image` aspect ratio.
- Popular fixes:
    - remove the `height` (or `width` );
    - Set `height` to `auto`;
    - HTML images

        ```css
        img {
          object-fit: cover; 
          /* object-fit: `contain`; */
        }
        ```

    - CSS images

        ```css
        div {
          /* Some other bg properties might needed to get this to work. */
          background-size: cover; 
        }
        ```

--- 

## Friday reflection
### Learning Objectives
- Walkthrough: [Tony's GH home page](https://acidtone.github.io/)
- Practice process (see below).
- Plan out some cards.

### Coding process
1. Understand the problem
    - Goal?
2. Plan it out
    - split the problem (aka. divide and conquer)
    - inside-out or outside-in?
3. Brute force a solution
    - dirty code is great
    - stay focused on the problem
    - take breaks
    - problem solved? `git commit`
4. Walk-through
    - `git status`
    - what was the goal again?
    - todo: add todos
    - document side projects but stay on target
5. Optimize
    - start with simple bits
6. Clean-up and prep
    - `git commit`
    - optional: `git push`
    - Revisit Step 1, proceed to Step 2.

---

## Open lab-time
1. Understand the problem
2. What mode are you in? 
    - Brute Force
    - Walk-through
    - Optimization

---

## Dailies
- Submit today's Codepen/repo/gist to the Dailies section (in Assessments) in Brightspace.