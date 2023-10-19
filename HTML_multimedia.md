## Multimedia formats

### Video formats
Only MP4, WebM, and Ogg video are supported by the HTML standard.


`MPEG (.mpg, .mpeg)`

MPEG. Developed by the Moving Pictures Expert Group. The first popular video format on the web. Not supported anymore in HTML.


`AVI (.avi)`	

AVI (Audio Video Interleave). Developed by Microsoft. Commonly used in video cameras and TV hardware. Plays well on Windows computers, but not in web browsers.


`WMV (.wmvW)`

MV (Windows Media Video). 
Developed by Microsoft. Commonly used in video cameras and TV hardware. Plays well on Windows computers, but not in web browsers.


`QuickTime (.mov)`

QuickTime. Developed by Apple. Commonly used in video cameras and TV hardware. Plays well on Apple computers, but not in web browsers.


`RealVideo	(.rm, .ram)`

RealVideo. Developed by Real Media to allow video streaming with low bandwidths. Does not play in web browsers.


`Flash	(.swf,.flv)`	

Flash. Developed by Macromedia. Often requires an extra component (plug-in) to play in web browsers.


`Ogg (.ogg)`

Theora Ogg. Developed by the Xiph.Org Foundation. Supported by HTML.


`WebM (.webm)`	

WebM. Developed by Mozilla, Opera, Adobe, and Google. Supported by HTML.


`MPEG-4 or MP4 (.mp4)`

MP4. Developed by the Moving Pictures Expert Group. Commonly used in video cameras and TV hardware. Supported by all browsers and  recommended by YouTube. 

### The HTML `<video>` element is used to show a video on a web page.

```
<!DOCTYPE html>
<html>
<body>

<video width="320" height="240" controls>
  <source src="doc-files/niko.mp4" type="video/mp4"> 
  <source src="doc-files/niko.webm" type="video/webm">
</video>

</body>
</html>
```

`controls` attribute adds video controls, like play, pause, and volume.

It is a good idea to always include width and height attributes

`<source>` element allows you to specify alternative video files which the browser may choose from. The browser will use the first recognized format.

```
<video width="320" height="240" controls>
  <source src="doc-files/niko.mp4" type="video/mp4">
  <source src="doc-files/niko.webm" type="video/webm">
</video>
```

### `<video>` autoplay

```
<!DOCTYPE html>
<html>
<body>

<video width="320" height="240" autoplay>
  <source src="doc-files/niko.mp4" type="video/mp4">
  <source src="doc-files/niko1.ogg" type="video/ogg">
</video>

</body>
</html>
```

! Chromium browsers do not allow autoplay in most cases. However, muted autoplay is always allowed.

### `<muted>` `<autoplay>` 

Add muted after autoplay to let your video start playing automatically (but muted):

```
<!DOCTYPE html>
<html>
<body>

<video width="320" height="240" autoplay muted>
  <source src="doc-files/niko.mp4" type="video/mp4">
  <source src="doc-files/niko.webm" type="video/webm">
  Your browser does not support the video tag.
</video>

</body>
</html>
```

### HTML Video - Methods, Properties, and Events


The HTML DOM defines methods, properties, and events for the `<video>` element.

This allows you to load, play, and pause videos, as well as setting duration and volume.
```
<!DOCTYPE html> 
<html> 
<body> 

<div style="text-align:center"> 
  <button onclick="playPause()">Play/Pause</button> 
  <button onclick="makeBig()">Big</button>
  <button onclick="makeSmall()">Small</button>
  <button onclick="makeNormal()">Normal</button>
  <br><br>
  <video id="video1" width="420">
    <source src="doc-files/niko.mp4" type="video/mp4">
    <source src="doc-files/niko.webm" type="video/webm">
    
  </video>
</div> 

<script> 
var myVideo = document.getElementById("video1"); 

function playPause() { 
  if (myVideo.paused) 
    myVideo.play(); 
  else 
    myVideo.pause(); 
} 

function makeBig() { 
    myVideo.width = 560; 
} 

function makeSmall() { 
    myVideo.width = 320; 
} 

function makeNormal() { 
    myVideo.width = 420; 
} 
</script> 

</body> 
</html>
```
![Alt text](doc-files/hm.png)

### audio formats
Only MP3, WAV, and Ogg audio are supported by the HTML standard.


`MIDI (.mid, .midi)`

MIDI (Musical Instrument Digital Interface). Main format for all electronic music devices like synthesizers and PC sound cards. MIDI files do not contain sound, but digital notes that can be played by electronics. Plays well on all computers and music hardware, but not in web browsers.


`RealAudio	(.rm, .ram)`

RealAudio. Developed by Real Media to allow streaming of audio with low bandwidths. Does not play in web browsers.


`WMA (.wma)`

WMA (Windows Media Audio). Developed by Microsoft. Plays well on Windows computers, but not in web browsers.


`AAC (.aac)`	

AAC (Advanced Audio Coding). Developed by Apple as the default format for iTunes. Plays well on Apple computers, but not in web browsers.


`WAV (.wav)`	

WAV. Developed by IBM and Microsoft. Plays well on Windows, Macintosh, and Linux operating systems. Supported by HTML.


`Ogg (.ogg)`	

Ogg. Developed by the Xiph.Org Foundation. Supported by HTML.


`MP3 (.mp3)`	

MP3 files are actually the sound part of MPEG files. MP3 is the most popular format for music players. Combines good compression (small files) with high quality. Supported by all browsers.


`MP4 (.mp4)`	

MP4 is a video format, but can also be used for audio. Supported by all browsers.


### `<audio>` element is used to play an audio file on a web page.

```
<!DOCTYPE html>
<html>
<body>

<audio controls>
  <source src="doc-files/niko.ogg" type="audio/ogg">
  <source src="doc-files/niko.mpeg" type="audio/mpeg">
</audio>

</body>
</html>
```

`controls` attribute adds audio controls, like play, pause, and volume.

### `autoplay`

```
<!DOCTYPE html>
<html>
<body>

<audio controls autoplay>
  <source src="doc-files/niko.ogg" type="audio/ogg">
  <source src="doc-files/niko.mpeg" type="audio/mpeg">
</audio>

</body>
</html>
```
Chromium browsers do not allow autoplay in most cases. However, muted autoplay is always allowed.

### `muted`  `autoplay`

```
<!DOCTYPE html>
<html>
<body>

<audio controls autoplay muted>
  <source src="doc-files/niko.ogg" type="audio/ogg">
  <source src="doc-files/niko.mpeg" type="audio/mpeg">
</audio>

</body>
</html>
```

## `<object>` element

The `<object>` tag defines a container for an external resource.

The external resource can be a web page, a picture, a media player, or a plug-in application.

To embed a picture, it is better to use the `<img>` tag.

To embed HTML, it is better to use the `<iframe>` tag.

To embed video or audio, it is better to use the `<video>` and `<audio>` tags.

```
<!DOCTYPE html>
<html>
<body>

<object data="doc-files/chibi2.jpg"></object>
 
</body>
</html>
```

`<object>` can also be used to include HTML in HTML:

```
<object width="100%" height="500px" data="xyz.html"></object>
```



### `<embed>` element

`<embed>` element also defines an embedded object within an HTML document.

```
<!DOCTYPE html>
<html>
<body>

<embed src="doc-files/chibi2.jpg">
 
</body>
</html>
```

`<embed>` element can also be used to include HTML in HTML:

```
<embed width="100%" height="500px" src="xyz.html">
```

## Playing a YouTube Video in HTML


```
<!DOCTYPE html>
<html>
<body>

<iframe width="420" height="345" src="https://www.youtube.com/embed/w0AOGeqOnFY">
</iframe>

</body>
</html>
```


### `mute=1`  `autoplay=1`

Video start playing automatically but muted.

```
<!DOCTYPE html>
<html>
<body>

<iframe width="420" height="345" src="https://www.youtube.com/embed/w0AOGeqOnFY?autoplay=1&mute=1">
</iframe>

</body>
</html>
```
### `loop`

`loop=1` to let your video loop forever.

Value 0 (default): The video will play only once.

Value 1: The video will loop (forever).


```
<!DOCTYPE html>
<html>
<body>

<iframe width="420" height="345" src="https://www.youtube.com/embed/w0AOGeqOnFY?playlist=w0AOGeqOnFY&loop=1">
</iframe>

</body>
</html>
```

### `controls`


`controls=0` to not display controls in the video player.

Value 0: Player controls does not display.

Value 1 (default): Player controls display.

```
<!DOCTYPE html>
<html>
<body>

<iframe width="420" height="345" src="https://www.youtube.com/embed/w0AOGeqOnFY?controls=0">
</iframe>

</body>
</html>
```



