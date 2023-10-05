## HTML Colors

HTML colors are specified with predefined color names, or with RGB, HEX, HSL, RGBA, or HSLA values.

Color Converter


https://www.w3schools.com/colors/colors_converter.asp

### Color names 

Color Names Supported by All Browsers

https://www.w3schools.com/colors/colors_names.asp

Named Colors Sorted by HEX Value

https://www.w3schools.com/colors/colors_hex.asp

### Background Color

```
<!DOCTYPE html>
<html>
<body>

<h1 style="background-color:CornflowerBlue;">Hello World</h1>

<p style="background-color:SkyBlue;">
Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam nonummy nibh euismod tincidunt ut laoreet dolore magna aliquam erat volutpat.
Ut wisi enim ad minim veniam, quis nostrud exerci tation ullamcorper suscipit lobortis nisl ut aliquip ex ea commodo consequat.
</p>

</body>
</html>
```
![Alt text](doc-files/Screenshot_2023-09-30_at_13.11.25.png)

### Text Cloor

```
<!DOCTYPE html>
<html>
<body>

<h3 style="color:SteelBlue;">Hello World</h3>

<p style="color:DodgerBlue;">Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam nonummy nibh euismod tincidunt ut laoreet dolore magna aliquam erat volutpat.</p>

<p style="color:SkyBlue;">Ut wisi enim ad minim veniam, quis nostrud exerci tation ullamcorper suscipit lobortis nisl ut aliquip ex ea commodo consequat.</p>

</body>
</html>
```
![Alt text](doc-files/Screenshot_2023-09-30_at_13.16.40.png)

### Border Color

```
<!DOCTYPE html>
<html>
<body>

<h1 style="border: 2px solid DarkTurquoise;">Hello World</h1>

<h1 style="border: 2px solid DarkCyan;">Hello World</h1>

<h1 style="border: 2px solid Aquamarine;">Hello World</h1>

</body>
</html>
```
![Alt text](doc-files/Screenshot_2023-09-30_at_13.21.01.png)

```
<!DOCTYPE html>
<html>
<body>

<p>Same as color name "Blue":</p>

<h1 style="background-color:rgb(0, 0, 255);">rgb(0, 0, 255)</h1>
<h1 style="background-color:#0000FF;">#0000FF</h1>
<h1 style="background-color:hsl(240, 100%, 50%);">hsl(240, 100%, 50%)</h1>

<p>Same as color name "Blue", but 50% transparent:</p>
<h1 style="background-color:rgb(0, 0, 255,0.5);">rgb(0, 0, 255,0.5)</h1>
<h1 style="background-color:hsl(240, 100%, 50%,0.5);">hsl(240, 100%, 50%,0.5)</h1>

<p>In addition to the predefined color names, colors can be specified using RGB, HEX, HSL, or even transparent colors using RGBA or HSLA color values.</p>

</body>
</html>
```
![Alt text](doc-files/Screenshot_2023-09-30_at_17.09.58.png)


## HTML RGB, RGBA colors

An `RGB` color value represents `RED`, `GREEN`, and `BLUE` light sources.

An `RGBA` color value is an extension of RGB with an Alpha channel (opacity).

## RGB

An RGB color value is specified with:

red, 

green, 

blue.


Each parameter defines the intensity of the color with a value between 0 and 255

For example, rgb(255, 0, 0) is displayed as `red`, because `red` is set to its highest value (255), and the other two (green and blue) are set to 0. 

To display `black`, set all color parameters to 0, like this: rgb(0, 0, 0).

To display `white`, set all color parameters to 255, like this: rgb(255, 255, 255).

```
<!DOCTYPE html>
<html>
<body>

<h1 style="background-color:rgb(255, 0, 0);">rgb(255, 0, 0)</h1>
<h1 style="background-color:rgb(0, 0, 255);">rgb(0, 0, 255)</h1>
<h1 style="background-color:rgb(0, 255, 0);">rgb(0, 255, 0)</h1>
<h1 style="background-color:rgb(0, 0, 0);">rgb(0, 0, 0)</h1>
<h1 style="background-color:rgb(255, 255, 255);">rgb(255, 255, 255)</h1>


</body>
</html>
```
![Alt text](doc-files/Screenshot_2023-09-30_at_14.04.00.png)

### RGBA

An RGBA color value is specified with:

red, 

green, 

blue, 

alpha.

The alpha parameter is a number between 0.0 fully transparent and 1.0 not transparent

```
<!DOCTYPE html>
<html>
<body>

<h1 style="background-color:rgba(0, 0, 250, 0);">rgba(0, 0, 250, 0)</h1>
<h1 style="background-color:rgba(0, 0, 250, 0.2);">rgba(0, 0, 250, 0.2)</h1>
<h1 style="background-color:rgba(0, 0, 250, 0.4);">rgba(0, 0, 250, 0.4)</h1>
<h1 style="background-color:rgba(0, 0, 250, 0.6);">rgba(0, 0, 250, 0.6)</h1>
<h1 style="background-color:rgba(0, 0, 250, 0.8);">rgba(0, 0, 250, 0.8)</h1>
<h1 style="background-color:rgba(0, 0, 250, 1);">rgba(0, 0, 250, 1)</h1>

</body>
</html>
```
![Alt text](doc-files/Screenshot_2023-09-30_at_14.15.13.png)

## HTML HEX Colors

#rrggbb

Where rr (red), gg (green) and bb (blue) are hexadecimal values between 00 and ff (same as decimal 0-255).

#ff0000 is displayed as `red`, because `red` is set to its highest value (ff), and the other two (green and blue) are set to 00.

#00ff00 is displayed as `green` and 
#0000ff is `blue`

To display `black`, set all color parameters to 00, like this: #000000.

To display `white`, set all color parameters to ff, like this: #ffffff.

```
<!DOCTYPE html>
<html>
<body>

<h1 style="background-color:#ff0000;">#ff0000</h1>
<h1 style="background-color:#00ff00;">#00ff00</h1>
<h1 style="background-color:#0000ff;">#0000ff</h1>


</body>
</html>
```
![Alt text](doc-files/Screenshot_2023-09-30_at_16.09.00.png)

## HTML HSL and HSLA Colors

### HSL

An HSL color value is specified with:

hue, 

saturation, 

lightness. 


`Hue` is a degree on the color wheel from 0 to 360. 

0 is `red`, 

120 is `green`, and 

240 is `blue`.

`Saturation` is a percentage value. 

0% means a shade of gray, and 

100% is the full color.

`Lightness` is also a percentage value. 

0% is `black`, and 

100% is `white`.

```
<!DOCTYPE html>
<html>
<body>

<h1 style="background-color:hsl(0, 100%, 50%);">hsl(0, 100%, 50%)</h1>
<h1 style="background-color:hsl(240, 100%, 50%);">hsl(240, 100%, 50%)</h1>
<h1 style="background-color:hsl(120, 100%, 50%);">hsl(120, 100, 50%)</h1>
<h1 style="background-color:hsl(0, 0%, 0%);">hsl(0, 0%, 0%)</h1>
<h1 style="background-color:hsl(0, 0%, 100%);">hsl(0, 0%, 100%)</h1>

</body>
</html>
```
![Alt text](doc-files/Screenshot_2023-09-30_at_16.48.05.png)

### HSLA

An HSLA color value is specified with:

hue, 

saturation, 

lightness, 

alpha.

```
<!DOCTYPE html>
<html>
<body>

<h1 style="background-color:hsla(240, 100%, 50%, 0);">hsla(240, 100%, 50%, 0)</h1>
<h1 style="background-color:hsla(240, 100%, 50%, 0.2);">hsla(240, 100%, 50%, 0.2)</h1>
<h1 style="background-color:hsla(240, 100%, 50%, 0.4);">hsla(240, 100%, 50%, 0.4)</h1>
<h1 style="background-color:hsla(240, 100%, 50%, 0.6);">hsla(240, 100%, 50%, 0.6)</h1>
<h1 style="background-color:hsla(240, 100%, 50%, 0.8);">hsla(240, 100%, 50%, 0.8)</h1>
<h1 style="background-color:hsla(240, 100%, 50%, 1);">hsla(240, 100%, 50%, 1)</h1>

</body>
</html>
```
![Alt text](doc-files/Screenshot_2023-09-30_at_16.54.37.png)

