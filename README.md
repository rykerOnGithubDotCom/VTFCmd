# VTFCmd
VTFCmd is a C command line frontend for VTFLib that can create VTF and VMT files from various file formats created by Neil Jedrzejewski.



## Correct VTFCmd usage:
```
 -file <path>             (Input file path.)
 -folder <path>           (Input directory search string.)
 -output <path>           (Output directory.)
 -prefix <string>         (Output file prefix.)
 -postfix <string>        (Output file postfix.)
 -version <string>        (Ouput version.)
 -format <string>         (Ouput format to use on non-alpha textures.)
 -alphaformat <string>    (Ouput format to use on alpha textures.)
 -flag <string>           (Output flags to set.)
 -resize                  (Resize the input to a power of 2.)
 -rmethod <string>        (Resize method to use.)
 -rfilter <string>        (Resize filter to use.)
 -rsharpen <string>       (Resize sharpen filter to use.)
 -rwidth <integer>        (Resize to specific width.)
 -rheight <integer>       (Resize to specific height.)
 -rclampwidth <integer>   (Maximum width to resize to.)
 -rclampheight <integer>  (Maximum height to resize to.)
 -gamma                   (Gamma correct image.)
 -gcorrection <single>    (Gamma correction to use.)
 -nomipmaps               (Don't generate mipmaps.)
 -mfilter <string>        (Mipmap filter to use.)
 -msharpen <string>       (Mipmap sharpen filter to use.)
 -normal                  (Convert input file to normal map.)
 -nkernel <string>        (Normal map generation kernel to use.)
 -nheight <string>        (Normal map height calculation to use.)
 -nalpha <string>         (Normal map alpha result to set.)
 -nscale <single>         (Normal map scale to use.)
 -nwrap                   (Wrap the normal map for tiled textures.)
 -bumpscale <single>      (Engine bump mapping scale to use.)
 -nothumbnail             (Don't generate thumbnail image.)
 -noreflectivity          (Don't calculate reflectivity.)
 -shader <string>         (Create a material for the texture.)
 -param <string> <string> (Add a parameter to the material.)
 -recurse                 (Process directories recursively.)
 -exportformat <string>   (Convert VTF files to the format of this extension.)
 -silent                  (Silent mode.)
 -pause                   (Pause when done.)
 -help                    (Display vtfcmd help.)
```

  

## Example VTFCmd usage:

```
vtfcmd.exe -file "C:\texture1.bmp" -file "C:\texture2.bmp" -format "dxt1"
vtfcmd.exe -file "C:\texture.bmp" -format "bgr888" -normal -postfix "normal_"
vtfcmd.exe -folder "C:\input\*.tga" -output "C:\output" -recurse -pause
vtfcmd.exe -folder "C:\output\*.vtf" -output "C:\input" -exportformat "jpg"
```

  

## Windows

1. Download VTFCmd from the Releases page.
2. Execute the VTFCmd.exe using the Windows command prompt (tip: try typing cmd in the file path box).

  

## Linux

1. Download VTFCmd from the Releases page.
2. Download [Wine](https://wiki.winehq.org/Download).
3. Execute VTFCmd using Wine as shown below:

​		`wine VTFCmd.exe [options]`

  

## Resources

[Nem's Tools Website](https://nemstools.github.io/)
