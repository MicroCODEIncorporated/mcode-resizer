# mcode-resizer
A pair of C# .NET classes that enable any Windows Form to automatically resize to any DPI at any Scale on any display.


## Description

After adding these two .NET C# classes to any Windows Forms project any Form can be updated to auto-size<br>
by editing just three (3) lines of code.

The auto-sizing of these classes does not rely on any Windows features, no DPI scaling mode, no anchoring<br>
of controls, etc. It relies on Windows display properties and math alone to retain the best possible appearance<br>
of all controls in a Windows Form for all possible resolutions, scales, and shapes. It also supports dynamic scaling<br>
changes and dragging between display of different capabilities.


## Using the MicroCODE.Resizer


### Dependencies

* Reference these two C# Classes ('Resizer.cs' and 'ResizerForm.cs') in your project

* Set The Properties on your Form to "AutoScaleMode = None" -- 'Resizer' will take care of it all

        //
        // AppScreen
        //
        this.AutoScaleMode = System.Windows.Forms.AutoScaleMode.None;


* Change your Forms to inherit "ResizerForm" (which itself inherits "Form") instead of "Form" directly

        // Inherit from 'ReserForm' for display independence
        public partial class AppScreen : ResizerForm, IAppScreen, IAppEvents
        {

* Call "UseResizer()" after "IntializeComponents()" -- this method is included in "Reszier.cs"


        // Use MicroCODE's auto-scaling / auto-resizing capability...
        UseResizer(parentForm: this);


### Installing

Clone this repo and copy these files into your Visual Studio project:
- ResizerForm.cs
- Resizer.cs

<p align="left"><img src=".\images\resizer-files.png" width="512" title="MicroCODE Resizer Files..."></p>

* Change your Forms to inherit 'ResizerForm' instead of 'System.Windows.Form'
* Call 'UseResizer()' immediately after 'InitializeComponents()'
<br>
<br>

### Demonstration of the MicroCODE Resizer...

<video id="demo-video" style="border-style:solid; border-width:2px" src="https://user-images.githubusercontent.com/8990676/158492176-6917b8ce-2b35-4b26-9e87-8886f31f3998.mp4" width="1024" allowfullscreen="allowfullscreen" webkitallowfullscreen="webkitallowfullscreen" mozallowfullscreen="mozallowfullscreen" allow="autoplay *" loop autoplay autobuffer controls muted>
Your browser does not support the HTML5 player.
</video>
</p>
<br>
<br>

## Help

This is delivered AS-IS under the MIT License, but we will make every effort to<br>
address any issues you may find to improve the Resizer. If you have improvements<br>
or suggests to contribute clone this repository and give us a pull request with<br>
your documentation.<br>
<br>


## Terminology

| Word or Acronym	| Description/Definition                                |
|-------------------|-------------------------------------------------------|
|  Resizer	        | Our class and process for permanent resolution independence.
|  Scale            | The user selected scaling of the Windows displays.
|  DPI              | Dots per Inch - where the default is 96 dpi.
|  High DPI         | A monitor supports more than 96 dpi.
|  DPI Aware        | An application that can scale itself regardless of DPI.
|                   | The MicroCODE.Resizer adds 'DPI Awareness' to your App.
|  -
|  PXPI             | Pixels per Inch
|  PTPI             | Points per Inch
|  PXPP             | Pixels per Point
|  IPPT             | Inches per Point
|  IPPX             | Inches per Pixel
|  PTPP             | Points per Pixel
|  -
|  STANDARD         | Measurements, ratios, and sizes associated with a 96 dpi monitor.
|  NATIVE           | Measurements, ratios, and sizes associated with physical monitor.
|  DISPLAY          | Measurements, ratios, and sizes associated with the 'Scaled' display on the physical monitor.


## Authors

Contributors names and contact info:

* Timothy J McGuire [@tjmcode](https://tjmcode.github.io/)



## Release History

* 0.0
    * Initial release of our internal code for use by others.

## Future Development

* 0.1
    * Improve Child Form awareness of Parent Form resizing.


## License

This project is licensed under the MIT License - see the LICENSE.md file for details
