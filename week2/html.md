# HTML Quick Reference

A short reference of the HTML commands learned so far.

| Tag / Command   | Meaning                                | Example                           |
| --------------- | -------------------------------------- | --------------------------------- |
| `<h1>` – `<h6>` | Headings, from highest to lowest level | `<h1>Hello</h1>`                  |
| `<p>`           | Paragraph                              | `<p>Hello World</p>`              |
| `<a>`           | Creates a link                         | `<a href="url">Google</a>`        |
| `<ol>`          | Ordered/numbered list                  | `<ol>...</ol>`                    |
| `<ul>`          | Unordered/bullet list                  | `<ul>...</ul>`                    |
| `<li>`          | List item                              | `<li>Java</li>`                   |
| `<strong>`      | Strong importance; usually bold        | `<strong>Important</strong>`      |
| `<em>`          | Emphasized text; usually italic        | `<em>Hello</em>`                  |
| `<b>`           | Bold text without semantic importance  | `<b>Bold</b>`                     |
| `<i>`           | Alternate voice/style; usually italic  | `<i>Italic</i>`                   |
| `<br>`          | Line break                             | `Hello<br>World`                  |
| `<hr>`          | Thematic horizontal separation         | `<hr>`                            |
| `<div>`         | Generic block-level container          | `<div>Content</div>`              |
| `<span>`        | Generic inline container               | `<span>Text</span>`               |
| `<img>`         | Displays an image                      | `<img src="pic.jpg" alt="Photo">` |
| `<form>`        | Creates a form                         | `<form>...</form>`                |
| `<label>`       | Label for a form control               | `<label>Name</label>`             |
| `<input>`       | Creates an input field                 | `<input type="text">`             |
| `<button>`      | Creates a button                       | `<button>Submit</button>`         |
| `<textarea>`    | Multi-line text input                  | `<textarea></textarea>`           |
| `<select>`      | Creates a dropdown                     | `<select>...</select>`            |
| `<option>`      | Option inside a dropdown               | `<option>Java</option>`           |
| `<table>`       | Creates a table                        | `<table>...</table>`              |
| `<tr>`          | Table row                              | `<tr>...</tr>`                    |
| `<th>`          | Table header cell                      | `<th>Name</th>`                   |
| `<td>`          | Table data cell                        | `<td>John</td>`                   |
| `<header>`      | Header section                         | `<header>...</header>`            |
| `<nav>`         | Navigation section                     | `<nav>...</nav>`                  |
| `<main>`        | Main page content                      | `<main>...</main>`                |
| `<section>`     | Groups related content                 | `<section>...</section>`          |
| `<article>`     | Independent content                    | `<article>...</article>`          |
| `<aside>`       | Side/related content                   | `<aside>...</aside>`              |
| `<footer>`      | Footer section                         | `<footer>...</footer>`            |

## Important Attributes

| Attribute     | Meaning                        | Example                     |
| ------------- | ------------------------------ | --------------------------- |
| `href`        | Link destination               | `href="https://google.com"` |
| `target`      | Where the link opens           | `target="_blank"`           |
| `src`         | Source of an image/resource    | `src="image.jpg"`           |
| `alt`         | Alternative text for an image  | `alt="Profile photo"`       |
| `id`          | Unique identifier              | `id="username"`             |
| `class`       | Groups elements for styling/JS | `class="button"`            |
| `name`        | Name of a form control         | `name="email"`              |
| `value`       | Value of an input/control      | `value="Java"`              |
| `placeholder` | Hint inside an input           | `placeholder="Enter name"`  |
| `required`    | Makes a field required         | `required`                  |
| `disabled`    | Disables an element            | `disabled`                  |

## Common Input Types

```html
<input type="text">
<input type="password">
<input type="email">
<input type="number">
<input type="date">
<input type="checkbox">
<input type="radio">
<input type="file">
<input type="submit">
```

## Basic HTML Structure

```html
<!DOCTYPE html>
<html>
<head>
    <title>My Page</title>
</head>

<body>

    <!-- Page content -->

</body>
</html>
```

> **Note:** `<eu>` is not a standard HTML tag. Unknown/custom tags don't have built-in HTML meaning.
