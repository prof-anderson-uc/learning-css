# Learning CSS

This repository contains the starter files for a Web Design 1 coding exercise introducing the basics of CSS.

In earlier exercises, you focused mostly on HTML. HTML gives a web page structure and meaning. CSS, or Cascading Style Sheets, controls the visual presentation of that content.

In this exercise, you'll begin learning how to change the appearance of a web page by writing CSS rules. You will practice changing colors, fonts, spacing, borders, backgrounds, and page layout. You'll also learn the difference between **internal** style sheets and **external** style sheets.

This is a follow-along coding exercise. Watch the videos in Canvas in order, pause when needed, and type the code yourself in Visual Studio Code.

---

## Use Canvas for the Full Assignment Instructions

Canvas has the full assignment description, screencast videos, due date, and submission instructions.

This GitHub repository is where the starter files are stored.

For this exercise, you are **not** making your own GitHub repository (yet).

You are **not** using a template repository.

You are **not** cloning the repository.

You are **not** committing or pushing anything to GitHub.

For this exercise, you are only downloading the starter files as a ZIP file, editing them on your computer, zipping your completed folder, and submitting the completed ZIP file in Canvas.

---

## Important: Download the ZIP File

For this exercise, use GitHub only as a place to download the starter files.

The basic workflow is:

1. Go to the GitHub repository.
2. Click the green **Code** button.
3. Choose **Download ZIP**.
4. Save the ZIP file to your computer.
5. Unzip the folder before working.
6. Open the unzipped folder in Visual Studio Code.
7. Complete the coding exercise.
8. Zip the completed folder.
9. Submit the completed ZIP file in Canvas.

Do **not** work directly inside the ZIP file. You must unzip it first.

---



## Recommended Folder Organization

Before you start coding, put the unzipped project folder somewhere organized.

A good setup would be to create one main folder for this course, then place each coding exercise inside it.

Example:

- 📁`web-design-1`
  - 📁`handsome`
  - 📁`learning-html`
  - 📁`hollow-earth`
  - 📁`learning-css`

Keeping your files organized will make your life much easier as the course continues. Web projects depend on exact file names and folder locations, so losing track of files can cause broken links, missing images, missing CSS, and other problems.

After you unzip the starter files, you may delete the original ZIP file so you do not confuse it with the completed ZIP file you will submit later.

---

## A Short Introduction to CSS

CSS stands for Cascading Style Sheets.

HTML describes what the content is.

CSS describes how that content should look.

For example:

- HTML can say “this is the main heading.”
- CSS can say “make the main heading dark green, larger, centered, and spaced away from the content below.”

CSS works by selecting HTML elements and declaring how they should change.

A basic CSS rule has three major parts:

- a selector
- a property
- a value

The selector chooses what you want to change.

The property identifies what aspect you want to change.

The value tells the browser what you want that property to become.

Example:

- `h1 { color: olive; }`

In that example:

- `h1` is the selector
- `color` is the property
- `olive` is the value

---

## Internal Style Sheets

In the early videos, you will write CSS inside the HTML file using the `<style>` element.

This is called an **internal** style sheet.

An internal style sheet is placed inside the `<head>` of the HTML document.

Internal style sheets are useful when you are learning because everything is in one file and you can see the connection between the HTML and CSS more easily.

However, internal style sheets only affect that one page. They are not the best choice for larger websites with multiple pages.

---

## External Style Sheets

Later in the exercise, you will move toward using **external** style sheets.

An external style sheet is a separate CSS file that gets linked to an HTML page.

External style sheets are the standard approach for real websites because many pages can share the same CSS file.

That means if you want to change the design of the website, you can update one CSS file instead of changing the same style rules on every HTML page.

You will learn how to connect an external CSS file using the `<link>` element.

---

## Reset Style Sheets

The exercise also introduces a **reset style sheet**.

Browsers automatically apply default styles to HTML elements. For example, headings are large and bold, paragraphs have spacing, lists are indented, and body content may have default margins.

Those defaults can be helpful, but they can also make CSS confusing when you are learning.

A reset style sheet removes many of those browser defaults so you can start from a cleaner, more predictable baseline.

In this exercise, you will connect `reset.css` first, then connect your own CSS file after it.

The order matters.

The reset style sheet should come first because it removes default styling.

Your own style sheet should come second because it adds your design choices back in.

---

## CSS Syntax Reminders

CSS syntax is different from HTML syntax.

In HTML, you use angle brackets, tags, attributes, and closing tags.

In CSS, you use selectors, curly braces, properties, values, colons, and semicolons.

A typical CSS rule looks like this:

- `selector { property: value; }`

As your CSS gets more complex, it is easier to write each property on its own line:

- `selector {`
- `  property: value;`
- `  property: value;`
- `}`

This makes the code easier to read and easier to troubleshoot.

---

## Semicolons Matter

Each CSS declaration should end with a semicolon.

Example:

- `color: red;`

The semicolon tells the browser that one declaration is finished and another can begin.

If you forget a semicolon, the next declaration may not work correctly.

This is one of the most common beginner CSS mistakes.


---

## Important Concepts to Remember

### CSS changes appearance, not meaning

HTML describes the structure and meaning of content.

CSS changes how that content looks.

Try to keep those two jobs separate.

### Selectors choose what to style

A selector tells the browser which elements should pay attention to a CSS rule.

Common selector types include:

- element selectors
- class selectors
- descendant selectors
- grouped selectors

### Declarations say what changes

Inside the curly braces, declarations tell the browser what to change.

Each declaration has a property and a value.

Example:

- `color: crimson;`

### The cascade matters

CSS stands for Cascading Style Sheets.

That means styles can inherit, combine, override, and build on one another.

The order of rules and the relationship between elements can affect what appears in the browser.

### File order matters

When linking multiple CSS files, the order matters.

For this exercise, the reset style sheet should come before your own style sheet.

That way, the reset removes default browser styling first, and your own CSS adds your chosen design afterward.

---

## Before You Submit

Before submitting your work in Canvas, check the following:

- Your project folder is unzipped
- Your project folder is saved somewhere you can find it
- You opened the full project folder in Visual Studio Code
- You watched the videos in order
- You saved your files
- Your internal style sheet examples work
- Your class selector examples work
- Your box model styles are visible
- Your `header` and `main` elements are in the correct places
- Your reset style sheet is linked correctly
- Your own external CSS file is linked correctly
- The reset style sheet is linked before your own CSS file
- Your wrapper is added correctly
- Your page looks correct when previewed in a browser
- You zipped the entire completed project folder, not just one file

---

## What to Submit

When you are finished, compress the entire completed project folder into a ZIP file and submit that ZIP file in Canvas.

Do not submit only one HTML file.

Do not submit only your CSS file.

This project depends on multiple files working together. If you submit only one file, the project may not work correctly when it is opened on another computer.

---

## Troubleshooting Tips

If something is not working, check these common issues first.

### My CSS is not changing anything

Check:

- Did you save the file?
- Is your CSS inside the `style` element if you are using an internal style sheet?
- Is your external CSS file linked correctly?
- Is the file name spelled correctly?
- Is the CSS file in the same folder that your `href` path expects?
- Did you forget a semicolon?
- Did you forget a closing curly brace?

### My page looks like the reset broke everything

That is normal at first.

A reset style sheet removes many browser defaults. Headings may no longer be large, lists may look strange, and spacing may disappear.

The reset gives you a clean slate. Your own CSS adds the design back in.

### My list numbers or bullets disappeared

They may not actually be gone.

A reset style sheet may remove the default spacing around lists, causing bullets or numbers to sit off the edge of the page.

Once you add your own margin or padding, they will become visible again.

### My class selector is not working

Check:

- In CSS, did you start the class selector with a period?
- In HTML, did you use the `class` attribute?
- Are the class names spelled exactly the same way?
- Did you use quotation marks around the class value?

For example:

- CSS: `.big-red`
- HTML: `class="big-red"`

### My background color changed but my text is hard to read

You may have created a contrast problem.

If the background is dark, the text usually needs to be light.

If the background is light, the text usually needs to be dark.

Remember that `background-color` controls the background, while `color` controls the text color.

### My external style sheet is not working

Check the `link` element.

Make sure your `href` points to the correct CSS file.

Also make sure your reset CSS is linked before your own CSS file.

### My wrapper is not centered

Check that the wrapper has a width and automatic left and right margins.

A common pattern is:

- `margin-left: auto;`
- `margin-right: auto;`

The wrapper also needs a width for auto margins to visibly center it.

---

## Final Reminder

CSS is where web pages start to feel more visual.

It can also feel picky at first. A missing semicolon, misspelled property, incorrect selector, or broken file path can stop a style from working.

That is normal.

The goal of this exercise is not to memorize every CSS property. The goal is to understand the basic pattern:

Select something.

Declare what should change.

Save the file.

Preview the result.

Adjust and test again.

The more you practice that process, the more natural CSS will become.
