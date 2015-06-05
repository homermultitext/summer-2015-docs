# Creating  a Codex Model #

Creating a codex model is an incredibly important task because it is the first step in creating a navigable manuscript. What you are doing is creating a set of relationships between the images and the folios themselves, and indicating the sequential order in which they appear. Without this work, the manuscripts would not be browsable in a sequential order. There are two kinds of URNs you will be using:

1. object URN refering to the image (as a concrete object)
2. object URN refering to the folio (as a concept)

Your codex model is contained within a simple comma-separated-values (csv) file. This file has five columns:

1. Folio: This is the URN for the folio as a concept
2. Sequence: numerically, what page is this?
3. RV: Indicate whether the page is a recto or verso
4. Label: This is the full attribution for the manuscript and where it comes from, what will change is the folio and side
5. Default Image: This is the URN for the image as a concrete object

**Folio URN Format** urn:cite:hmt:X.Y

- X is the siglum for the manuscript (such as msA for the Venetus A)
- Y is the folio side (such as 12r)

**Default Image URN** urn:cite:hmt:X_Y
- X is the siglum for the manuscript (such as msA for the Venetus A)
- Y is the unique identifier for each image, these will vary depending on the manuscript, but you will be given the data where you can check them.

