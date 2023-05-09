# CSS

## CSS is a language that describes the style of an HTML document.

### CSS describes how HTML elements should be displayed.

---

#### How to add CSS to HTML

##### There are three ways of inserting a style sheet:

1. Inline Styles

```html
<section style="background: red">
  <h1>Get the freedom you deserve.</h1>
</section>
```

- Inline styles are defined within the "style" attribute of the relevant element and are generally discouraged to use because they are not reusable and overrides styles declared in the <style> tag and external style sheets. They are written as a property followed by a colon and a value.

2. `<style>` tag

```html
<head>
  <meta charset="UTF-8" />
  <meta http-equiv="X-UA-Compatible" content="ie=edge" />
  <title>uHost</title>
  <link rel="shortcut icon" href="favicon.png" />
  <style>
    section {
      background: #ccc;
      padding: 20px;
      margin: 20px;
    }
  </style>
</head>
```

3. External Style Sheet

```html
<link rel="stylesheet" href="main.css" />
```

> main.css

```css
section {
  background: red;
  padding: 20px;
  margin: 20px;
}
```

- external stylesheets are reccomended because they can be cached by the browser, which improves page load speed, and they can be used by multiple HTML documents... if the styles are included in the HTML document, they have to be repeated in every HTML document that uses them.

---

### Google Fonts

[Google Fonts](https://fonts.google.com/) is a library of free licensed font families, an interactive web directory for browsing the library, and APIs for conveniently using the fonts via CSS and Android.

---

### CSS Selectors

- CSS selectors are used to "find" (or select) the HTML elements you want to style.

#### Universal Selector
- The universal selector (*) selects all HTML elements on the page.

```css
* {
  color: red;
}
```

#### Element Selector
- The element selector selects HTML elements based on the element name.

```css
p {
  color: red;
}
```
#### Class Selector
- The class selector selects HTML elements with a specific class attribute.

```css
.blue {
  color: blue;
}
```

#### ID Selector
- The id selector uses the id attribute of an HTML element to select a specific element.

```css
#green {
  color: green;
}
```

#### Attribute Selector
- The attribute selector selects HTML elements with a specific attribute value.

```css
a[target="_blank"] {
  background-color: yellow;
}
```

