## HTML Links
HTML links are defined with the `<a>` tag witch defines a hyperlink

`<a href="url">link text</a>`

The `href` attribute indicates the link's destination.

The link text is the part that will be visible to the reader.


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

### By default, links will appear as follows in all browsers:

- An unvisited link is underlined and blue
- A visited link is underlined and purple
- An active link is underlined and red

### HTML Links - The target Attribute

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


### Absolute URLs vs. Relative URLs

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


### HTML Links - Use an Image as a Link

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

