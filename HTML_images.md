## HTML Images

HTML images are defined with the `<img>` tag.

The source file `src`, alternative text `alt`, `width`, and `height` are provided as attributes

```
<!DOCTYPE html>
<html>
<body>

<h2>HTML Images</h2>
<p>HTML images are defined with the img tag:</p>

<img src="doc-files/chibi2.jpg" alt="chibi" width="300" height="300">

</body>
</html>
```
![Alt text](<doc-files/Screenshot 2023-10-03 at 14.13.47.png>)


```
<!DOCTYPE html>
<html>
<head>
<style>
/* This style sets the width of all images to 100%: */
img {
  width: 100%;
}
</style>
</head>
<body>

<h2>Width/Height Attributes or Style?</h2>

<p>The first image uses the width attribute (set to 128 pixels), but the style in the head section overrides it, and sets the width to 100%.</p>

<img src="doc-files/chibi2.jpg" alt="image" width="128" height="128">

<p>The second image uses the style attribute to set the width to 128 pixels, this will not be overridden by the style in the head section:</p>

<img src="doc-files/chibi2.jpg" alt="image" style="width:128px;height:128px;">

</body>
</html>
```

![Alt text](<doc-files/Screenshot 2023-10-03 at 14.12.01.png>)

## Images in Another Folder

```
<!DOCTYPE html>
<html>
<body>

<h2>Images in Another Folder</h2>
<p>It is common to store images in a sub-folder. You must then include the folder name in the src attribute:</p>

<img src="/Users/aris/Documents/20211224_165825.png" alt="HTML5 Icon" style="width:128px;height:128px;">

</body>
</html>
```
![Alt text](<doc-files/Screenshot 2023-10-03 at 14.09.53.png>)

## Images on Another Server

```
<!DOCTYPE html>
<html>
<body>

<h2>Images on Another Server</h2>

<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/1/15/Cat_August_2010-4.jpg/1920px-Cat_August_2010-4.jpg" alt="wikipedia.org" style="width:204px;height:142px;">

</body>
</html>
```
![Alt text](<doc-files/Screenshot 2023-10-03 at 11.49.29.png>)

## Animated Images

```
<!DOCTYPE html>
<html>
<body>

<h2>Animated Images</h2>

<p>HTML allows moving images:</p>

<img src="doc-files/2GU.gif" alt="computer cat" style="width:300px;height:300px;">

</body>
</html>
```
![Alt text](<doc-files/Screenshot 2023-10-03 at 11.56.20.png>)

## Floating Images

```
<!DOCTYPE html>
<html>
<body>

<h2>Floating Images</h2>
<p><strong>Float the image to the right:</strong></p>

<p>
<img src="doc-files/chibi2.jpg" alt="chibi" style="float:right;width:42px;height:42px;">
A paragraph with a floating image. A paragraph with a floating image. A paragraph with a floating image.
</p>

<p><strong>Float the image to the left:</strong></p>
<p>
<img src="doc-files/chibi2.jpg" alt="chibi" style="float:left;width:42px;height:42px;">
A paragraph with a floating image. A paragraph with a floating image. A paragraph with a floating image.  
</p>

</body>
</html>
```
![Alt text](<doc-files/Screenshot 2023-10-03 at 14.06.39.png>)

### Image Maps

The HTML `<map>` tag defines an image map. An image map is an image with clickable areas. The areas are defined with one or more `<area>` tags.


```
<!DOCTYPE html>
<html>
<body>

<h2>Image Maps</h2>
<p>Click on the paladin or octopus to go to a new page and read more about the topic:</p>

<img src="doc-files/rycerzs.jpg" alt="Github" usemap="#workmap" width="532" height="376">

<map name="workmap">
  <area shape="rect" coords="358,373,500,47" alt="paladin" href="http://git.artemi.uk/">
  <area shape="circle" coords="92,271,106" alt="octopus" href="http://git.artemi.uk/">
</map>

</body>
</html>
```

![Alt text](<doc-files/Screenshot 2023-10-03 at 15.43.25.png>)



### How to create a image map

1. Add to `<img>` tag `usemap`  value with a hash tag `#` followed by the name of the image map this create a relationship between the image and the image map.

2. Add `<map>` element with `name` atribute with the same name as usemap `#`

3. Add the clickable areas using `<area>` element 

4. Define the `shape` of the clikable area: 
- rect - defines a rectangular region
- circle - defines a circular region
- poly - defines a polygonal region
- default - defines the entire region

5. Define some `coordinates` to be able to place the clickable area onto the image. 

6. Add link to destination page in `href` attribute.




