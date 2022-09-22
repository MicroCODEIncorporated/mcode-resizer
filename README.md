# mcode-resizer
A pair of C# .NET classes that enable any Windows Form to automatically resize to any DPI at any Scale.


## Description

After adding these two .NET C# classes to any Windows Forms project any Form can be updated to auto-size
by editing just two (2) lines of code.

The auto-sizing of these classes does not rely on any Windows features, no DPI scaling mode, no anchoring
of controls, etc.


## Using the MicroCODE.Resizer


### Dependencies

* These two C# Classes must be added to your project
* ...{TO-DO}



### Installing

* Clone this repo and copy these files into your Visual Studio project:
- ResizerForm.cs
- Resizer.cs

<p align="left"><img src=".\images\resizer-files.png" width="512" title="MicroCODE Resizer Files..."></p>

* Change your Forms to inherit 'ResizerForm' instead of 'System.Windows.Form'


### Demonstration of the MicroCODE Resizer...

<video id="demo-video" style="border-style:solid; border-width:2px" src="https://user-images.githubusercontent.com/8990676/cannot-upload.mp4" width="1024" allowfullscreen="allowfullscreen" webkitallowfullscreen="webkitallowfullscreen" mozallowfullscreen="mozallowfullscreen" allow="autoplay *" loop autoplay autobuffer controls muted>
Your browser does not support the HTML5 player.
</video>
</p>



## Help

This is delivered AS-IS under the MIT License, but we will make every effort to
address any issues you may find to improve the Resizer. If you have improvements
or suggests to contribute clone this repository and give us a pull request with
your documentation.



## Terminology

| Word or Acronym	| Description/Definition                                |
|-------------------|-------------------------------------------------------|
|  Resizer	        | Our class and process for permanent resolution independence.
|  Scale            | The user selected scaling of the Windows displays.
|  DPI              | Dots per Inch - where the default is 96 dpi.
|  High DPI         | A monitor supports more than 96 dpi.
|  DPI Aware        | An application that can scale itself regardless of DPI.
|                   | The MicroCODE.Resizer adds 'DPI Awareness' to your App.


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
