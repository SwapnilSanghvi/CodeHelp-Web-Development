# Dot-Batch-Debug-Exercise-HTML

## 1. Add a "tooltip" to the paragraph below with the text "Dot Batch".

```html
<p tooltip="Dot Batch">Web Development Master Course</p>
```

### Solution

```html
<p title="Dot Batch">Web Development Master Course</p>
```

---

## 2. Add six headings to the document with the text "CodeHelp". Start with the most important heading (the largest) and end with the least important heading (the smallest).

```html
<html>
  <body>
    <p>CodeHelp</p>
    <p>CodeHelp</p>
    <p>CodeHelp</p>
    <p>CodeHelp</p>
    <p>CodeHelp</p>
    <p>CodeHelp</p>
  </body>
</html>
```

### Solution

```html
<html>
  <body>
    <h1>CodeHelp</h1>
    <h2>CodeHelp</h2>
    <h3>CodeHelp</h3>
    <h4>CodeHelp</h4>
    <h5>CodeHelp</h5>
    <h6>CodeHelp</h6>
  </body>
</html>
```

---

## 3. Complete this document with proper element end tags.

```html
<h1>
  This is a Heading
  <p>This is a paragraph.</p>
</h1>
```

### Solution

```html
<h1>This is a Heading</h1>
<p>This is a paragraph.</p>
```

---

## 4. Wrap this poem around such HTML tags that will preserve all spaces and line-breaks when the element is displayed.

```html
<poem>
  My house is red - a little house; A happy child am I: I laugh and play the
  whole day long, I hardly ever cry. I have a tree, a green, green tree, To
  shade me from the sun; And under it I often sit, When all my play is done.
</poem>
```

### Solution

```html
<pre>
    My house is red - a little house;
    A happy child am I:
    I laugh and play the whole day long,
    I hardly ever cry.

    I have a tree, a green, green tree,
    To shade me from the sun;
    And under it I often sit,
    When all my play is done.
</pre>
```

---

## 5. Use the HTML image attributes to set the size of the image to 250 pixels height and 400 pixels wide.

```html
<img src="https://bit.ly/3I7Q44c" />
```

### Solution

```html
<img src="https://bit.ly/3I7Q44c" width="250" height="400" />
```

---

## 6. Add a submit button to the form, and specify that it should go to "/submit.html".

```html
<form submit="/submit.html">
  Email: <input type="email" name="email" />
  <p>Submit</p>
</form>
```

### Solution

```html
<form action="/submit.html">
  Email: <input type="email" name="email" />
  <p>Submit</p>
</form>
```
