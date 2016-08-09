Creating your own emblems
Emblems are simply squared images that the game sticks on top of a background to create a flag.

Custom Flag Example
For each emblem 3 texture files in the Direct Draw Texture format (.dds) are required: a default, medium-sized one; a big one, usually white and displayed only on the galactic map; and a small one displayed next to units.

It is recommended to add the emblems using mods instead of placing them directly in the game folder to avoid any possible problems. Here's more information on how to create them and where are they can be found.

The textures should follow these specifications:

All textures must be located in a subfolder of <mod_root>/flags/.
All three textures should have the same file name, for example, emblem.dds
The default texture should have a size of 128 X 128 pixels and should be in the folder <mod_root>\flags\<folder>\
The map texture should have a size of 256 X 256 pixels and should be in the folder <mod_root>\flags\<folder>\map\
The small texture should have a size of 24 x 24 pixels and should be in the folder <mod_root>\flags\<folder>\small\

Guide[edit]
Create a mod using the Stellaris Launcher.
Create a folder named 'flags' in the root folder, and a subfolder that you can name however you want in it, this folder is where all the textures files will be placed.
Create 'usage.txt' in the subfolder with the following contents, it will prevent AI empires from using the emblem in their flags (savegames will still work once you remove the mod):
    random = no 
    show_in_designer = yes
Create a folder named 'localisation' in the root folder. You must place there localisation (.yml) files, otherwise the category you made for the emblem won't have a name! This is an example for the english translation, the name after 'FLAG_CATEGORY' must match the name of the new folder you created under flags:
   l_english:
   
     FLAG_CATEGORY_new_flags:0 "New Flags!"
Create your emblem! Remember that it should be a square image and that it is best to create out your image with a transparent back drop.
Now you need to generate the 3 texture files out of the image: the medium, large and small ones. Remember that they have to be .dds files and have to have determinate size each one. You can use GIMP with the .dds plugin, Photoshop with the NVIDIA plugin, ImageMagick, Paint.NET with the .dds plugin and others to convert your images to textures.
Now place the medium texture in the folder you created under 'flags', create the folders 'map' and 'small' and place the big and small textures in each one, respectively, the folder structure should be like this now:
   new_mod/
   +-- flags
   ¦   +-- new_flags
   ¦       +-- emblem.dds
   ¦       +-- usage.txt
   ¦       +-- map
   ¦       ¦   +-- emblem.dds
   ¦       +-- small
   ¦           +-- emblem.dds
   +-- localisation
       +-- new_mod_l_braz_por.yml
       +-- new_mod_l_english.yml
       +-- new_mod_l_french.yml
       +-- new_mod_l_german.yml
       +-- new_mod_l_polish.yml
       +-- new_mod_l_russian.yml
       +-- new_mod_l_spanish.yml
   
   5 directories, 11 files
Special Considerations:

Texture compression: Using DXT1 or DXT5 compression may introduce artifacts in the textures, use uncompressed textures (ARGB 8888) if this happens.
Remember that the game recolors your image when showing it. Some colors may be distorted when you view your flags from the galaxy map.