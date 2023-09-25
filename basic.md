## Documents
1. All HTML documents must start with a document type declaration: `<!DOCTYPE html>`

2. The HTML document itself begins with `<html>` and ends with `</html>`.

3. The visible part of the HTML document is between `<body>` and `</body>`.

```
<!DOCTYPE html>
<html>
<body>

<h1>My First Heading</h1>

<p>My first paragraph.</p>

</body>
</html>
```

### `<!DOCTYPE>`

The `<!DOCTYPE>` declaration represents the document type, and helps browsers to display web pages correctly.

It appear once, at the top of the page, is not case sensitive (so you could write it in lowercase, if you wanted to. But as the official documents use the capitalized doctype. => You can write it the way you want, but I recommend writing it in uppercase letters.)

The `<!DOCTYPE>` declaration for HTML5 is: `<!DOCTYPE html>`

### HTML Headings `<h1>`

HTML headings are defined with the `<h1>` to `<h6>` tags.

`<h1>` - most important heading
`<h6>` - the least important heading
```
<!DOCTYPE html>
<html>
<body>

<h1>This is heading 1</h1>
<h2>This is heading 2</h2>
<h3>This is heading 3</h3>
<h4>This is heading 4</h4>
<h5>This is heading 5</h5>
<h6>This is heading 6</h6>

</body>
</html>
```
![Alt text](doc-files/b2.png)

### HTML Paragraphs `<p>`
```
<!DOCTYPE html>
<html>
<body>

<p>paragraph1.</p>
<p>paragraph2.</p>

</body>
</html>
```
![Alt text](doc-files/b3.png)

### HTML Links
HTML links are defined with the `<a>` tag

```
<!DOCTYPE html>
<html>
<body>

<h2>HTML Links</h2>
<p>HTML links are defined with the a tag:</p>

<a href="http://git.artemi.uk/">Link to my git</a>

</body>
</html>

```
![Alt text](doc-files/b4.png)


### HTML Images

HTML images are defined with the `<img>` tag.

The source file `src`, alternative text `alt`, `width`, and `height` are provided as attributes

```
<!DOCTYPE html>
<html>
<body>

<h2>HTML Images</h2>
<p>HTML images are defined with the img tag:</p>

<img src="/Users/aris/Desktop/cat.jpg" alt="kotek" width="453" height="605">

</body>
</html>

```
![Alt text](<doc-files/Screenshot 2023-09-25 at 16.40.36.png>)

