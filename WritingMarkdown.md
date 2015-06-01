# Writing Markdown #

We like to do our scholarly writing in markdown, a simple writing style that is more versatile than traditional editors, like Microsoft Word, and simpler than more complicated writing styles like XML.

## The Basics ##

### Paragraphs ###

In order to distinguish between paragraphs, you simply have to leave at least one line of white space, much as you might distinguish between paragraphs in an email if you weren't indenting.

For example, with a space in between, this a new paragraph.

As is this.

And this.

### Headings ###

In order to create headings and subheadings we use '#'. Main headings use one '#' and each subsequent level adds a '#'. So for instance the the raw markdown the above headings look like this:

   # Writing Markdown #
  
   ## The Basics ##
   
   ### Paragraphs ###
   
   ### Headings ###

### Ordered Lists ###

You may want to create ordered lists, that is numbered lists. You can do those with simple number and period format. No matter what number you put, markdown will start the list with 1.

Here is an example of a list in the raw:

   2. Stuff
   3. Things
   7. Items

And the same markdown through an editor will produce this:

2. Stuff
3. Things
7. Items

### Unordered Lists ###

To create bulleted lists, you use the minus sign '-' followed by a space. Indenting will create a second level of bullets, like so:

- stuff
- things
- items
  - subitems
  
### Linking ###

Markdown has an easy way to incorporate links such as [the HMT website](www.homermultitext.org).

In raw markdown that link looks like this:

   [the HMT website](www.homermultitext.org)

If you have a lot of links in your document or links you repeat frequently, you may not want to have them written out that each time. You can also format link similar to foot notes. The raw markdown would look like this:

   [the HMT website][link1]
   
   [link1]: www.homermultitext.org

The first set of square brackets is a label for the link. It is what will show up in your prose. The second set of square brackets is a lable for the reference. These should be unique, but you can format them in any way you wish as long at they are contained in square brackets. Every time you want to use that same link, you use the same reference label, but the label that goes in your prose can change.

### Embedding Images ###

The formating for embedding images is very similar to linking, only you add an '!' in front of your square brackets and the file name of the image goes into the parantheses. Like so:

   ![pretty image](prettyimage.jpg)

## Slide Presentations ##

You can easily insert breaks to create slides within a markdown file by using three or more underscores '_'. In a regular text file these will create page breaks.

There are several pieces of software out there to convert markdown into slide presentations. We like mdpress, available [here](http://egonschiele.github.io/mdpress/).

## Advanced Writing ##

Some of your more advance writing might require more complicated functions. Here are some useful ones.

### Footnotes ###

In your prose if you want to insert a footnote you format them with square brackets, a carat, and an unique label. Much like linking there is then a corresponding note following by a colon and the contents you want in the footnote. Here is an example of what it looks like:

   I want to reference something.[^fn1]
   
   [^fn1]: and that something is written about down here.

### Tables ###

Generating tables is surprisingly easy, although there are many formating modifications you can make. Items in a table are separated by '|'. You'll need a label row and a divider row to start you off. The divider row should contain at least 3 '-'. You can include ':' to align material in a whole column (one side for right or left, both for center alignment).

Here is an example of a table in the raw:

   | Column A | Column B|
   |:---:|:---:|
   | item 1a | item 1b |
   | item 2a | item 2b |

And through a parser it looks like this:

| Column A | Column B|
|:---:|:---:|
| item 1a | item 1b |
| item 2a | item 2b |
