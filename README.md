# gsMeshUtilities

Open-Souce (MIT License) command-line utilities for mesh things.

Currently just one tool, in C#, but there is more to come, and probably there will be some C++ too...

Questions? Contact Ryan Schmidt [@rms80](http://www.twitter.com/rms80) / [gradientspace](http://www.gradientspace.com)


# General Notes

You can find pre-built windows executables in the top-level **builds** folder.


# sdkmeshToOBJ

Microsoft has released some awesome mesh-processing tools under the MIT license, in 
particular https://github.com/Microsoft/UVAtlas is a fantastic tool for auto-generating UV maps for
unstructured triangle meshes. However, this tool only outputs a weird *.sdkmesh* format that almost
no other tool supports. So, *sdkmeshToOBJ* converts this format to a standard OBJ with UV-coordinates.

Usage: **sdkmeshToOBJ.exe** *your_file.sdkmesh*

Output is **file.sdkmesh.obj**

Current Limitations: only the first mesh in the sdkmesh file is converted. And, it appears that sdkmesh files can contain multiple vertex buffers for a single mesh, but that isn't supported either.


