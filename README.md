# ImMultiText

ImMultiText is **single** header stream style extention for [ImGui](https://github.com/ocornut/imgui) text function.

Example

![Example](https://i.postimg.cc/4NBvk8mV/image.png)

Usage

    		ImMultiText::text() << ImColor(255,0,255,255) << "First line " << ImMultiText::endl <<
				ImColor(0,255,255,255) << getFont("Verdana", 18) << "Second line " <<
				getFont("Verdana", 14) << ImMultiText::endl << ImColor(255,0,0,255) << "Third line" <<
				ImMultiText::Image(myImage, ImVec2(15,15)) << " << thats a image";

## Features

 - Combine strings with integers, floats, doubles and more !
 - You can use multiple fonts and colors without any manual cleanup ,it pops everything itself.
 - Simple to modify and display the data you like with your own classes / structures.
 - You can even display images along side your text !

## How to use
Make sure to include ImMultiText.h

First you must retrieve an instance of MultiText by calling ImMultiText like so:

    ImMultiText()

Then you simply use the << operator to append the functionality you like, options include:

    << [color] /*supports ImColor and ImVec4*/;
    
    << [text] /*supports const char* and strings*/;
    
    << [number value] /*supports int, double, float and various more*/;
    
    << [font] /*supports ImFont**/;
    
    << ImMultiText::Image(IDirect3DTexture9* image, ImVec2 size);
    
    << ImMultiText::endl /*creates a new line*/;
    
    << ImMultiText::setPrecision(int) /*sets the precision for floating point numbers);
    
## discord 
PEPPAPEEPO#3123
