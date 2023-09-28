## Documents
1. All HTML documents must start with a document type declaration: `<!DOCTYPE html>`

2. The HTML document itself begins with `<html>` and ends with `</html>`.

3. The visible part of the HTML document is between `<body>` and `</body>`.


The `<html>` element is the root element and it defines the whole HTML document.

It has a start tag `<html>` and an end tag `</html>`

Then, inside the `<html>` element there is a `<body>` element

The `<body>` element defines the document's body.

It has a start tag `<body>` and an end tag `</body>`

Then, inside the `<body>` element there are two other elements: `<h1>` and `<p>`

The `<h1>` element defines a heading.

It has a start tag `<h1>` and an end tag `</h1>`


The `<p>` element defines a paragraph.

It has a start tag `<p>` and an end tag `</p>`

```
<!DOCTYPE html>
<html>
<body>

<h1>My First Heading</h1>

<p>My first paragraph.</p>

</body>
</html>
```
### HTML Comment Tag
```
<!DOCTYPE html>
<html>
<body>

<!-- This is a comment -->
<p>This is a paragraph.</p>
<!-- Comments are not displayed in the browser -->

</body>
</html>
```
![Alt text](<doc-files/Screenshot 2023-09-28 at 16.49.55.png>)

```
<!DOCTYPE html>
<html>
<body>

<p>Paragraph.</p>

<!-- <p>Hidden paragraph </p> -->

<p>Paragraph too.</p>

</body>
</html>
```
![Alt text](<doc-files/Screenshot 2023-09-28 at 16.54.12.png>)


```
<!DOCTYPE html>
<html>
<body>

<p>Paragraph.</p>
<!--
<p>Look at this cool image:</p>
<img border="0" src="https://beks.pl/wp-content/uploads/2017/09/AE73_lowres.jpg" alt="Beksiński">
-->
<p>Paragraph.</p>

</body>
</html>
```

## `<!DOCTYPE>`

The `<!DOCTYPE>` declaration represents the document type, and helps browsers to display web pages correctly.

It appear once, at the top of the page, is not case sensitive (so you could write it in lowercase, if you wanted to. But as the official documents use the capitalized doctype. => You can write it the way you want, but I recommend writing it in uppercase letters.)

The `<!DOCTYPE>` declaration for HTML5 is: `<!DOCTYPE html>`


## `<html>`

### `lang`

Add `lang` attribute inside the `<html>` tag, to declare the language of the Web page. This is meant to assist search engines and browsers.
```
<!DOCTYPE html>
<html lang="en">
<body>

<h1>My First Heading</h1>

<p>My first paragraph.</p>

</body>
</html>
```
Country codes can also be added to the language code in the `lang` attribute.

`<html lang="en-US">`

## `<body>`

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

### Specify the size for any heading with the style attribute, using the CSS font-size property:
```
<!DOCTYPE html>
<html>
<body>

<h1 style="font-size:60px;">Bigger Heading</h1>

<p>You can change the size of a heading with the style attribute, using the font-size property.</p>

</body>
</html>
```
![Alt text](doc-files/b9.png)



### HTML Paragraphs `<p>`
```
<!DOCTYPE html>
<html>
<body>

<h2>Headling</h2>
<p>paragraph</p>
<p>paragraph</p>

</body>
</html>
```
![Alt text](doc-files/b3.png)


### HTML `style`

The HTML style attribute has the following syntax:

`<tagname style="property:value;">`

```
<!DOCTYPE html>
<html>
<body>

<p>black</p>
<p style="color:red;">red</p>
<p style="color:blue;">blue</p>
<p style="font-size:50px;">size</p>

</body>
</html>
```
![Alt text](doc-files/s1.png)

```
<!DOCTYPE html>
<html>
<body style="background-color:powderblue;">

<h1>Background color</h1>
<p>is blue</p>

</body>
</html>
```
![Alt text](<doc-files/Screenshot 2023-09-27 at 17.03.17.png>)

```
<!DOCTYPE html>
<html>
<body>

<h1 style="background-color:blue;">Heading</h1>
<p style="background-color:yellow;">Paragraph</p>

</body>
</html>
```
![Alt text](<doc-files/Screenshot 2023-09-27 at 17.08.09.png>)


```
<!DOCTYPE html>
<html>
<body>

<h1 style="color:pink;">Heading</h1>
<p style="color:purple;">Paragraph</p>

</body>
</html>
```
![Alt text](<doc-files/Screenshot 2023-09-27 at 17.11.05.png>)

```
<!DOCTYPE html>
<html>
<body>

<h1 style="font-family:verdana;">Font style 1</h1>
<p style="font-family:courier;">Font style 2</p>

</body>
</html>
```
![Alt text](<doc-files/Screenshot 2023-09-27 at 17.15.22.png>)

```
<!DOCTYPE html>
<html>
<body>

<h1 style="font-size:300%;">Font size 1</h1>
<p style="font-size:160%;">Font size 2</p>

</body>
</html>
```
![Alt text](<doc-files/Screenshot 2023-09-27 at 17.17.49.png>)

```
<!DOCTYPE html>
<html>
<body>

<h1 style="text-align:center;">Centered Heading</h1>
<p style="text-align:center;">Centered paragraph.</p>

</body>
</html>
```
![Alt text](<doc-files/Screenshot 2023-09-27 at 17.19.15.png>)


### HTML Horizontal 
The `<hr>` element is used to separate content (or define a change) in an HTML page:

The `<hr>` tag is an empty tag it has no end tag.
```
<!DOCTYPE html>
<html>
<body>

<h1>This is heading 1</h1>
<p>This is some text.</p>
<hr>

<h2>This is heading 2</h2>
<p>This is some other text.</p>
<hr>

<h2>This is heading 2</h2>
<p>This is some other text.</p>

</body>
</html>

```
![Alt text](doc-files/b10.png)


### Title

The `title` attribute defines some extra information about an element.

```
<!DOCTYPE html>
<html>
<body>

<h2 title="tooltip">Title</h2>

<p title="tooltip">Mouse over this paragraph, to display the title attribute as a tooltip.</p>

</body>
</html>
```
![Alt text](doc-files/b6.png)

### Single and Double Quotes

`<p title="John 'ShotGun' Nelson">`

![Alt text](doc-files/b7.png)

`<p title='John "ShotGun" Nelson'>`

![Alt text](doc-files/b8.png)

## `<br>`

HTML elements with no content are called empty elements.


The `<br>` tag defines a line break, and is an empty element without a closing tag:

```
<!DOCTYPE html>
<html>
<body>

<h1>My First Heading</h1>

<p>My first paragraph.</p>

<p>This is a <br> paragraph with a line break.</p>

</body>
</html>
```
![Alt text](doc-files/b5.png)

Use `<br>` if you want a line break (a new line) without starting a new paragraph:



``` 
<!DOCTYPE html>
<html>
<body>

<p>This is<br>a paragraph<br>with line breaks.</p>

</body>
</html>
```

![Alt text](doc-files/b11.png)

## `<pre>`


```
<!DOCTYPE html>
<html>
<body>

<p>The pre tag preserves both spaces and line breaks:</p>

<pre>
    The house cat sits
    And smiles and sings.
    He knows a lot 
    Of secret things.
</pre>

</body>
</html>
```
![Alt text](doc-files/b12.png)

### HTML Formatting Elements

Formatting elements were designed to display special types of text:

`<b>` - Bold text

`<strong>` - Important text

`<i>` - Italic text

`<em>` - Emphasized text

`<mark>` - Marked text

`<small>` - Smaller text

`<del>` - Deleted text

`<ins>` - Inserted text

`<sub>` - Subscript text

`<sup>` - Superscript text


```
<!DOCTYPE html>
<html>
<body>

<p>Normal text</p>

<p><b>Bold text</b></p>

<p><strong>Important text!</strong></p>

<p><i>Italic text</i></p>

<p><em>Emphasized text</em></p>

<p><small>Smaller text</small></p>

<p>Example of <mark>marked</mark> text.</p>

<p>Example of <del>deleted</del> text</p>

<p>Example of <del>deleted</del> <ins>inserted</ins> tekst.</p>

<p>This is <sub>subscripted</sub> text.</p>

<p>This is <sup>superscripted</sup> text.</p>


</body>
</html>

```

![Alt text](<doc-files/Screenshot 2023-09-28 at 13.27.17.png>)

### HTML `<blockquote>` for Quotations

```
<!DOCTYPE html>
<html>
<body>

<p>Here is a quote from SEIKO's website:</p>

<blockquote cite="https://www.seikowatches.com/global-en/special/heritage/">
    The story of Seiko began in 1881, when a 21 year old entrepreneur, Kintaro Hattori, opened a shop selling and repairing watches and clocks in central Tokyo. Today, after more than 130 years of innovation, Kintaro Hattori’s company is still dedicated to the perfection that the founder always strove to achieve. On the following pages you can explore Seiko’s long history and see many of our landmark watches.
</blockquote>

</body>
</html>
```
![Alt text](<doc-files/Screenshot 2023-09-28 at 14.19.55.png>)

### HTML `<q>` for Short Quotations

```
<!DOCTYPE html>
<html>
<body>

<p>Browsers usually insert quotation marks around the q element.</p>

<p>WWF's goal is to: <q>Build a future where people live in harmony with nature.</q></p>

</body>
</html>
```
![Alt text](<doc-files/Screenshot 2023-09-28 at 14.25.10.png>)

### HTML `<abbr>` for Abbreviations

Use the global title attribute to show the description for the abbreviation/acronym when you mouse over the element. 

```
<!DOCTYPE html>
<html>
<body>

<p>The <abbr title="World Health Organization">WHO</abbr> was founded in 1948.</p>

<p>Marking up abbreviations can give useful information to browsers, translation systems and search-engines.</p>

</body>
</html>
```
![Alt text](<doc-files/Screenshot 2023-09-28 at 14.30.15.png>)

### HTML `<address>` for Contact Information

The `<address>` element usually renders in italic, and browsers will always add a line break before and after the `<address>` element.



```
<!DOCTYPE html>
<html>
<body>

<p>The HTML address element defines contact information (author/owner) of a document or article.</p>

<address>
Written by John Doe.<br> 
Visit us at:<br>
Example.com<br>
Box 564, Disneyland<br>
USA
</address>

</body>
</html>
```

![Alt text](<doc-files/Screenshot 2023-09-28 at 14.38.42.png>)

### HTML `<cite>` for Work Title

```
<!DOCTYPE html>
<html>
<body>

<p>The HTML cite element defines the title of a work.</p>
<p>Browsers usually display cite elements in italic.</p>

<img src="https://beks.pl/wp-content/uploads/2017/09/AE73_lowres.jpg" width="220" height="277" alt="No Name">
<p><cite>No Name</cite> by Zdzisław Beksiński. Painted in 1973.</p>

</body>
</html>
```
![Alt text](<doc-files/Screenshot 2023-09-28 at 15.07.00.png>)


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

### HTML `<bdo>` 

BDO stands for Bi-Directional Override.

```
<!DOCTYPE html>
<html>
<body>

<p>If your browser supports bi-directional override (bdo), the next line will be written from right to left (rtl):</p>

<bdo dir="rtl">This line will be written from right to left</bdo>

</body>
</html>
```
![Alt text](<doc-files/Screenshot 2023-09-28 at 16.33.00.png>)


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

