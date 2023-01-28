# Explore

## Universal Selector

The universal selector is a special type selector and can therefore be namespaced when using @namespace. This is useful when dealing with documents containing multiple namespaces such as HTML with inline SVG or MathML, or XML that mixes multiple vocabularies.

```css
* {
  margin: 0;
  padding: 0;
}
```

---

## Nested Selector

Just like in HTML where you can have elements nested inside other elements, the same can be done in CSS. There are cases where you might want to style elements differently depending on what they are nested inside of. This is where nesting comes in handy.

> Descendant selector : When you want to target elements that are inside another element, you can use the descendant selector, also known as the descendant selector.

```css
main p {
  font-size: 1rem;
}
```

> Child Selector : For the cases where you only want to target direct children (nested only one level under), you can use a child selector. Instead of using a space, you use a greater-than character to specify direct children:

```css
main > p {
  font-size: 1rem;
}
```

> Adjacent Sibling Selector : There will sometimes be cases where you want to target an element based on whether or not it came right after another element.
> Let's say you wanted the first paragraph after every h1 tag to be in a larger font size:

```css
h1 + p {
  font-size: 125%;
}
```

---

## Attribute Selector

It is possible to style HTML elements that have specific attributes or attribute values.

> CSS `[attribute]` Selector : The `[attribute]` selector is used to select elements with a specified attribute.
> The following example selects all `<a>` elements with a target attribute:

```css
a[target] {
  background-color: yellow;
}
```

> CSS `[attribute="value"]` Selector : The `[attribute="value"]` selector is used to select elements with a specified attribute and value.
> The following example selects all `<a>` elements with a target="\_blank" attribute:

```css
a[target="_blank"] {
  background-color: yellow;
}
```

---

# Explore

## Font family

The font-family property specifies the font for an element.

The font-family property can hold several font names as a "fallback" system. If the browser does not support the first font, it tries the next font.

```css
p {
  font-family: "Times New Roman", Times, serif;
}
```

---

## Font weight

The font-weight CSS property sets the weight (or boldness) of the font. The weights available depend on the font-family that is currently set.

```css
/* Keyword values */
font-weight: normal;
font-weight: bold;

/* Keyword values relative to the parent */
font-weight: lighter;
font-weight: bolder;

/* Numeric keyword values */
font-weight: 100;
font-weight: 200;
font-weight: 300;
font-weight: 400; /* normal */
font-weight: 500;
font-weight: 600;
font-weight: 700; /* bold */
font-weight: 800;
font-weight: 900;
```

---

## Font style

The font-style CSS property sets whether a font should be styled with a normal, italic, or oblique face from its font-family.

```css
font-style: normal;
font-style: italic;
font-style: oblique;
font-style: oblique 10deg;
```

---

## Emphasis & Important

The text-emphasis property is used to apply emphasis marks to text.

The text-emphasis property is a shorthand for setting text-emphasis-style and text-emphasis-color in one declaration.

```css
p {
  text-emphasis: none|filled|open|dot|circle|double-circle|triangle|sesame|string|color;
}
```

## How to add external fonts

### Step 1: Download the font

Find the custom font you want to use on your website, and then download the TrueType Font file format (.ttf). You can also download the OpenType Font format (.otf)

---

### Step 2: Create a WebFont Kit for cross-browsing

Upload your .ttf or .otf file to the Webfont Generator and then download your Web Font Kit.

---

### Step 3: Upload the font files to your website

Using your FTP or file manager, upload all the font files found within your Web Font Kit to your website.\* Typically this kit will include multiple file extensions such as (.eot), (.woff), (.woff2), (.ttf) and (.svg).

Your kit will also include a Cascading Style Sheet (.css) that you will need to update and upload in step 4.

\*This step will vary greatly based upon how your website is built and hosted.

---

### Step 4: Update and upload your CSS file

Open the CSS file in a text editor such as Textedit, NotePad or Sublime.

Replace the existing source URL with the new URL you created by uploading each file.

By default, the source URL location is set within the downloaded Web Font Kit. It needs to be replaced by the location on your server.

Here’s a quick example:

Before update:

```css
@font-face {
  font-family: "CustomFont";
  src: url("CustomFont.eot");
  src: url("CustomFont.woff") format("woff"), url("CustomFont.otf") format("opentype"),
    url("CustomFont.svg#filename") format("svg");
}
```

After update:

```css
@font-face {
  font-family: "CustomFont";
  src: url("https://yoursite.com/css/fonts/CustomFont.eot");
  src: url("https://yoursite.com/css/fonts/CustomFont.woff") format("woff"), url("https://yoursite.com/css/fonts/CustomFont.otf")
      format("opentype"),
    url("https://yoursite.com/css/fonts/CustomFont.svg#filename") format("svg");
}
```

Once you’ve updated the CSS file, you need to upload it to your website (server).

---

### Step 5: Use the custom font in your CSS declarations

Now that your Cascading Style Sheet and font files are uploaded to your server, you can start using your custom font in your CSS declarations to help improve the look of the HTML.

This can be done in multiple ways, including adding site-wide declarations to your main CSS file.

Here is a quick example:

```css
h1 {
  font-family: "CustomFont", Arial, sans-serif;
  font-weight: normal;
  font-style: normal;
}
```

---

# Let suppose you have a div with 100px width and height. what happend if you will write 1000 words in this div?

> Content of div will overflow.

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <style>
      div {
        height: 100px;
        width: 100px;
        background-color: yellow;
      }
    </style>
  </head>
  <body>
    <div>
      Lorem ipsum, dolor sit amet consectetur adipisicing elit. Quas soluta, quo
      doloremque nesciunt ad illum suscipit, possimus fugit ducimus itaque
      repellendus alias aliquam ousdam? Rerum eius magnam similique veritatis
      quas repellendus consn ratione possimus assumenda praesentium beatae velit
      commodi.
    </div>
  </body>
</html>
```

---

# Clone following card

![Course Card](./course-card.png)

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Document</title>
    <link rel="preconnect" href="https://fonts.googleapis.com" />
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
    <link
      href="https://fonts.googleapis.com/css2?family=Rubik:wght@400;700&display=swap"
      rel="stylesheet"
    />
    <style>
      body {
        font-family: "Rubik", sans-serif;
      }
      .card {
        height: 377px;
        width: 400px;
        border: 1px solid black;
        padding: 20px;
      }
      img {
        width: 100%;
        border-radius: 10px;
      }
      h1 {
        font-size: 24px;
        width: 80%;
        line-height: 32px;
        letter-spacing: -0.6px;
      }
      hr {
        border-top: 1px solid rgb(237 237 237);
        opacity: 0.2;
      }
      p {
        font-size: 16px;
        line-height: 24px;
        font-weight: 800;
      }
      .price {
        color: #6674cc;
      }
      .label {
        background-color: #1dd1a1;
        color: #ffffff;
        padding: 5px;
        border-radius: 5px;
      }
      .price,
      strike {
        margin-right: 15px;
      }
    </style>
  </head>
  <body>
    <div class="card">
      <img src="./Web Development Master Course.jpeg" alt="" />
      <h1>Web Development Master Course @dot Batch</h1>
      <hr />
      <p>
        <span class="price">₹4500</span><strike>6999</strike
        ><span class="label">43% off</span>
      </p>
    </div>
  </body>
</html>
```

---
