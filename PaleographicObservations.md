# How to Take Paleographic Observations #

At the start of a new folio side, your first step will be to take paleographic observations on the *Iliad* text and the scholia text.

## *he Process ##

1. You're going to take observations from the first line on the folio side.
2. Enter your observations in 'paleography.csv' file located in the 'collections' folder of your repository. 
3. The file contains four columns: Observation, TextUrn, Image, and Comments
4. Observation: This column contains URN object references to the paleographic observation. And will look something like this:

  urn:cite:op:hmtX.Y

The two changing variables are 'X' and 'Y.' 'X' will refer to the book number you are taking your observation from. 'Y' will be a unique identifier for the particular observation. It will probably be easiest to start with 1 and go up sequentially, but remember that they are not numbers, they are names.

5. TextUrn: This column contains the cts URN for the glyph you are citing. For example if you are citing an alpha in the Venetus A *Iliad* 18.1, the URN would look like this:

  urn:cts:greekLit:tlg0012.tlg001.msA:18.1@α 
  
Repeated characters will be followed by square brackets and the number of times the letter has appeared in that particular text URN. The first occurence gets no brackets and number. So for example the second alpha in the Venetus A *Iliad* 18.1 would be referenced as followed:

  urn:cts:greekLit:tlg0012.tlg001.msA:18.1@α[2] 
  
You should ignore punctuation. Ligatures (e.g. epsilon-iota) should be treated as one glyph. If your glyph has any diacritical marks (accents or breathings), include those in both the image (see below) and in your TextUrn. They do not factor in how to number multiples, ergo an alpha with a rough breathing and an alpha with a smooth breathing would be 1 and 2. 

Remember that the text URN will change for the scholia. It might look something like this:

  urn:cts:greekLit:tlg5026.msA.hmt:18.1@α 

Keep in mind that the reference to the scholion will change based on how you have indexed them.
  
6. Image: This column contains the ROI URNS for the glyphs generated using the image citation tool (ICT). If your glyph has any diacritical marks (accents or breathings), include those in the image. Remember that a ligature counts as once glyph. A good rule of thumb is that if you can't get two characters distinctly in a single image, you should index them together.

7. Notes: This column is for any extra notes you may want to make, such as there being a ligature. You do not have to include notes if there is nothing to report. 

8. For the *Iliad* you should follow this process for the full first line on a folio side.

9. For the scholia you should follow this process for the first forty glyphs of main scholia. If there are more than forty glyphs in the first scholion you should stop at forty. If there are less you should move on to a second scholion until you get forty. 
