yagv-ng
=======
Yet Another Gcode Viewer - next generation

A G-Code viewer for 3D printer slicer generated outputs.

![screenshot](data/screenshot.png)

---
## Origins

This software was derived from [yagv][1] (also see [here][2]), created by [jonathanw][3].
then modified into [yagv-ng][0] by  [FMMT666[0] 


---
## License

[CC BY 4.0, Attribution 4.0 International][6]

You are free to:

Share — copy and redistribute the material in any medium or format  
Adapt — remix, transform, and build upon the material for any purpose, even commercially.
  
The licensor cannot revoke these freedoms as long as you follow the license terms.
  

---
## News
### CHANGES 2021-06-18

    - ran '2to3' on the .py files to make them into python3 compatible code then corrected errors produced when attempting to run.
    - made Gcode  G0x instead of only Gx acceptable,  discarded all  Gcode starting with M, discarded Gcode starting with '('and '%'
    - mapped G2 and G3 onto G1 , accept I J K values but not using them ... didn check the actual effect on rounded corners.
    - code now needs to import RegEx.

### CHANGES 2016/01/12

    - initial upload of the "ng" version
    - full mouse/trackpad/touchpad and mouse modifier support
    - viewpoint can now be moved up and down
    - rotation is now performed around the center of the screen


---

---
## Requirements

  - Python 3 
  - pyglet  and re
   

Yagv-ng was tested under
  
  - Linux, Ubuntu 20.04  and MINT 20  (Ulyana)
  - Mac OS X Yosemite and El Capitan
  - Windows 7
  
but should work with all system, that support OpenGL and mouse or touchpad/trackpad 
support.


--- 
## Installation

Right now, yagv-ng does not require an installation.  
If Python and pyglet are installed, it can be run from any directory by
just executing "yagv-ng".
  
Notice that there aren't any dialogs for opening and loading files, hence  
yagv-ng should be executed from a command line, inside a terminal:
  
    ./yagv-ng yourfilename.gcode
    
    
### Linux

Python, as well as pyglet should be available via your distribution's
package management system.
  

[0]: https://github.com/FMMT666/yagv-ng
[1]: https://github.com/jonathanwin/yagv
[2]: http://www.thingiverse.com/thing:38118
[3]: http://www.thingiverse.com/jonathanw/about
[4]: https://www.python.org/
[5]: https://bitbucket.org/pyglet/pyglet
[6]: http://creativecommons.org/licenses/by/4.0/
