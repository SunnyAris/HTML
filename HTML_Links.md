## HTML Links
HTML links are defined with the `<a>` tag witch defines a hyperlink

`<a href="url">link text</a>`

The `href` attribute indicates the link's destination.

The link text is the part that will be visible to the reader.


Use the `target` attribute to define where to open the linked document

Use the `<img>` element (inside `<a>`) to use an image as a link

Use the `mailto:` scheme inside the `href` attribute to create a link that opens the user's email program




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

## Link Titles

```
<!DOCTYPE html>
<html lang="en-US">
<body>

<h2>Link Titles</h2>
<p>The title attribute specifies extra information about an element. The information is most often shown as a tooltip text when the mouse moves over the element.</p>
<a href="http://git.artemi.uk/" title="Go to My Github">Visit my Github</a>

</body>
</html>
```

![Alt text](<doc-files/Screenshot 2023-10-02 at 15.05.13.png>)



## HTML Links - The target Attribute

The `target` attribute specifies where to open the linked document.

The `target` attribute can have one of the following values:

`_self` - Default. Opens the document in the same window/tab as it was clicked

`_blank` - Opens the document in a new window or tab

`_parent` - Opens the document in the parent frame

`_top` - Opens the document in the full body of the window

```
<!DOCTYPE html>
<html>
<body>

<h2>The target Attribute</h2>

<a href="http://git.artemi.uk/" target="_blank">Visit My Github!</a> 

<p>If target = "_blank", the link will open in a new browser window or tab.</p>

</body>
</html>
```

![Alt text](<doc-files/Screenshot 2023-10-02 at 12.00.22.png>)


## Absolute URLs vs. Relative URLs

Absolute URL = full web address

Relative URL = link to a page located in the html folder on the current web site

```
<!DOCTYPE html>
<html>
<body>

<h2>Absolute URLs</h2>
<p><a href="https://github.com/SunnyAris/HTML">Github</a></p>

<h2>Relative URLs</h2>
<p><a href="HTML_Links.md">HTML Links</a></p>

</body>
</html>
```


![Alt text](<doc-files/Screenshot 2023-10-02 at 13.10.19.png>)


## HTML Links - Use an Image as a Link

To use an image as a link put the `<img>` tag inside the `<a>` tag:

```
<!DOCTYPE html>
<html>
<body>

<h2>Image as a Link</h2>

<p>The image below is a link. Try to click on it.</p>

<a href="HTML_Links.md"><img src="doc-files/20211224_165825.png" alt="HTML" style="width:142px;height:142px;"></a>

</body>
</html>
```

![Alt text](<doc-files/Screenshot 2023-10-02 at 14.34.50.png>)


## Link to an Email Address


```
<!DOCTYPE html>
<html>
<body>

<h2>Link to an Email Address</h2>

<p>To create a link that opens in the user's email program (to let them send a new email), use mailto: inside the href attribute:</p>

<p><a href="mailto:someone@example.com">Send email</a></p>

</body>
</html>

```

![Alt text](<doc-files/Screenshot 2023-10-02 at 14.47.03.png>)

## Button as a link

To use an HTML button as a link, you have to add some JavaScript code.


```
<!DOCTYPE html>
<html>
<body>

<h2>Button as a Links</h2>

<p>Click the button to go to the HTML_Links</p>

<button onclick="document.location='HTML_Links.md'">HTML</button>

</body>
</html>
```

![Alt text](<doc-files/Screenshot 2023-10-02 at 14.52.48.png>)

## HTML Link Colors


An unvisited link is underlined and `blue`

A visited link is underlined and `purple`

An active link is underlined and `red`

You can change links colors, by using CSS:

```
<!DOCTYPE html>
<html>
<head>
<style>
a:link {
  color: green;
  background-color: transparent;
  text-decoration: none;
}
a:visited {
  color: blue;
  background-color: transparent;
  text-decoration: none;
}
a:hover {
  color: red;
  background-color: transparent;
  text-decoration: underline;
}
a:active {
  color: yellow;
  background-color: transparent;
  text-decoration: underline;
}
</style>
</head>
<body>

<h2 style="background-color:cornflowerblue;">Link Colors</h2>

<p style="background-color:skyblue;"> You can change the default colors of links</p>

<a href="http://git.artemi.uk/" target="_blank">My Github</a> 

</body>
</html>
```

![Alt text](<doc-files/Screenshot 2023-10-02 at 15.38.52.png>)


![Alt text](<doc-files/Screenshot 2023-10-02 at 15.39.35.png>)
