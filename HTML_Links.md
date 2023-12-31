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

![Alt text](doc-files/Screenshot_2023-10-02_at_15.05.13.png)



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

![Alt text](doc-files/Screenshot_2023-10-02_at_12.00.22.png)


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


![Alt text](doc-files/Screenshot_2023-10-02_at_13.10.19.png)


## HTML Links - Use an Image as a Link

To use an image as a link put the `<img>` tag inside the `<a>` tag:

```
<!DOCTYPE html>
<html>
<body>

<h2>Image as a Link</h2>

<p>The image below is a link. Try to click on it.</p>

<a href="HTML_Links.md"><img src="doc-files/chibi2.jpg" alt="HTML" style="width:142px;height:142px;"></a>

</body>
</html>
```

![Alt text](doc-files/Screenshot_2023-10-03_at_14.18.54.png)


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

![Alt text](doc-files/Screenshot_2023-10-02_at_14.47.03.png)


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

![Alt text](doc-files/Screenshot_2023-10-02_at_15.38.52.png)


![Alt text](doc-files/Screenshot_2023-10-02_at_15.39.35.png)


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

![Alt text](doc-files/Screenshot_2023-10-02_at_14.52.48.png)


### Link Buttons Color

```
<!DOCTYPE html>
<html>
<head>
<style>
a:link, a:visited {
  background-color: #6495ED;
  color: white;
  padding: 15px 25px;
  text-align: center;
  text-decoration: none;
  display: inline-block;
}

a:hover, a:active {
  background-color: blue;
}
</style>
</head>
<body>

<h2 style="color:SteelBlue;">Link Button</h2>
<p style="color:cornflowerblue;">A link styled as a button:</p>
<a href="http://git.artemi.uk/" target="_blank">Link Button</a>

</body>
</html>
```

![Alt text](doc-files/Screenshot_2023-10-02_at_15.58.16.png)

![Alt text](doc-files/Screenshot_2023-10-02_at_15.58.45.png)


## The HTML `<base>` element

The `<base>` element specifies the base URL and/or target for all relative URLs in a page.

The `<base>` tag must have either an href or a target attribute present, or both.

There can only be one single `<base>` element in a document!

```
<!DOCTYPE html>
<html>
<head>
  <base href="https://github.com/" target="_blank">
</head>
<body>

<h1>The base element</h1>

<p><img src="https://github.com/SunnyAris/HTML/raw/main/doc-files/Screenshot_2023-10-03_at_14.13.47.png" width="100" height="100" alt="chibi"> - Notice that we have only specified a relative address for the image. Since we have specified a base URL in the head section, the browser will look for the image at "https://github.com/SunnyAris/HTML/blob/main/HTML_images.md".</p>

<p><a href="SunnyAris/HTML/blob/main/HTML_images.md">HTML base tag</a> - Notice that the link opens in a new window, even if it has no target="_blank" attribute. This is because the target attribute of the base element is set to "_blank".</p>

</body>
</html>
```

![Alt text](doc-files/hl15.png)


