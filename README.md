# Purpose
The purpose of this is to:<br>
  A) Give me a project to work on<br>
  B) Provide a simple static site generator using python<br>
# Installation
Currently I do not have a PyPI package setup BUT you can install it from the following commands:<br>
`git clone https://github.com/RhinoCodes/Ebuilder-Ultra.git`<br>
`cd Ebuilder-Ultra && pip install setup.py`
* Note: I am not a pro at packaging stuff so be aware that the following commands may not work. 
   | If so feel free to start a Pull Request
 # Simple Usage
 This first simple example would create a .html file with a h1 tag, centered and gray.
  
 ```
 from ebuilder.ebuilder_core import *
 
 index = newpage('index')
 title = header(index, "Hello GitHub!")
 title.center()
 title.color('gray')
 index.commit()
 ```
  
```
from ebuilder.ebuilder_core import EbuilderTextComponent as etc
  
header_two = etc("h2")
```
This second simple example would create a new Text Component with the html tag h2 which for those of you unfamiliar with 
html is the second biggest size of text that is included without further styling (h1 being the first)

You can then call this like you would header, because they both use the EbuilderTextComponent class.

Note that if you only import EbuilderTextComponent you wont be able to 
access the other functions of Ebuilder Ultra, like making a new page, it is shown here
because it is the most efficient way.

# Advice Welcome
Feel free to dig through the source code and open Pull Requests and start issues, if you dig you'll see that EbuilderTextComponent 
has a bit of a weird implementation....
