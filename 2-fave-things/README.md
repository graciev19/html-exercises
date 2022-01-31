# 2-favorite-things

In this exercise, write a complete HTML page using elements discussed in the lecture, as well as from the readings.

Make the page about your favorite things! Don't worry about images yet, unless you understand how to implement them properly.

## Project Folder Setup

Within the root of this folder, `2-fave-things`, create the following within VS Code like we practiced during class:

- A new folder with your lastname
- Inside this folder, create an `index.html` file.

## Basic Webpage setup

Don't forget the basics: 

- `doctype`
- `html`
  - `head`
  - `body`

## `HEAD` elements

Practice adding metadata to your website with the following tags:

- `title`
- At least 3 `meta` tags. Refer to MDN or the link in my HTML lesson slides for some possible elements.

We'll be adding *resources*, such as `.css` files later this semester, so don't worry about them yet. 

## `BLOCK` elements

Practice structuring your page with some combination of nested `BLOCK` elements. Consider how to implement the following:

- `header`, `main`, `article`, `section`, `aside`, `footer`
- Meaningful heading tags at appropriate levels
- Common content block elements: 
  - paragraphs `p`
  - lists, such as `ul` or `ol` with nested list items (`li`)

Remember to refer to MDN or the HTML Board for help about when to use what element.

## `INLINE` elements

Practice wrapping inline text in your page by using the following `INLINE` elements:

- Use anchor tags `a` that link to other pages or parts of pages
  - `a` elements require the use of some *attributes*. Be sure to look them up.
- Use `strong` to wrap text that you wish to make more bold, 
- Use `em` where you want text to be emphasized via italics

## Tips on Versioning, Indentation, and Syntax

- Make sure your default spacing is set at 2
- Use your browser's inspection tool! See if it works, before you commit and push your work.
- Work on one part of your new page at a time. When you're done with that part, or need to stop working on it, commit your changes with a meaningful comment, and push them to the remote repo. This also means that your works is backed-up remotely too!
- Working on one part of a page at a time ensures that you spot
  - Appropriate opening and closing tags 
  - Using indentation to represent at what level an element is in the tree hierarchy

Here's a basic example with 2-spaced indentation below to help you remember. Note how everything is a nested within the `html`, the metadata `title` is within the `head`, the content is nested within the `body` (`header` > `body`, and `h1` > `header`).

```
<!doctype html>
<html lang="en">
  <head>
    <title>Example Indentation</title>
  </head>
  <body>
    <header>
      <h1>Example indentation</h1>
    </header>
  </body>
</html>
```
