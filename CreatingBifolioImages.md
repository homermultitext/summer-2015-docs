# Notes on creating images of bifolio spreads #

## Prerequisites: ##

1. install [GIMP](http://www.gimp.org/)
2. Set up

## Process: ##

3. Open GIMP
4. Select “File” then “New”
5. Set Width: 10000 px  Height: 7000 px. Ignore the warning about the size being too big.
6. Copy the verso image. Go to the archive of downloadable data and open the tif or jpeg file. Right click to copy image. 
7. In GIMP, select “Edit”, “Paste As”, and then “New Layer.”
8. Repeat for the recto image.
9. Using the rectangle drawing tool, select portions of the image you want to remove and cut them out (Command + X). You'll want to take from the center to match up the spines as close as you can. Save at least one of the color scales, ideally both. Avoid cutting from the top and bottom until you have the two images aligned.
10. Using the move tool align the images along the spine of the bifolio. 
11. Merge the layers into one: Under the 'Image' menu select 'Merge Visible Layers.' The default settings are acceptable. 
12. When you have merged the visible layers, using the rectangle tool again select the portion of the image that you want to keep. Now is the time to cut off any excess on the outside edges, but remember to keep at least one color scale. 
13. Copy this selection (Command + C).
14. Go the 'File' menu. Select 'Create' and then 'From Clipboard'.

## Saving: ##

14. Select “File” and “Save As”, and choose a place to save it where you will have easy access (desktop, a folder, etc.)
Name the file using the pattern: manuscript - verso number v- recto number r (e.g., gen49-10v-11r.xcf). This should create an .xcf file (still in GIMP).
In that same file, go to “File”, “Export” then select the location where the .xcf was saved, click “Export” in the saving window, and then click “Export” a final time in the new window which pops up. This should create a .png file with the same name.
