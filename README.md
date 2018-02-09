# useful-with-sigil
Some resources useful to creating an ebook with Sigil

## Introduction
__Sigil__ is a great tool for creating ebooks.
Unlike with the alternatives, you can edit
through either the WYSIWYG interface of the chapters that you create
or the XHTML source.
For a lot of workflows, ability to do this is un-negotiably essential.

However, unlike with some of the commercial alternatives,
setting up the basic structure of the book to a level that
is acceptable to ereaders in general isn't so simple.
This is a package of resources who's purpose is to make
that process a tad easier.

### Generate a Cover Page
According to [this site](http://www.ebookcoversize.com/),
an ebook cover should be a JPEG file of 1563 x 2500 pixels.

Use __GIMP__ (or another program) to create a file by these specs
by the name "CoverDesign.jpg". Then, add it to the Sigil project.

### Add the Cover Page
Add the file _resources/Text/CoverPage.xhtml_ to the Sigil project.
Then, you can delete that other XHTML file that was previously there.

Then make sure that the style-sheet referenced in the file is one that you plan to include.

### Replace the Metadata
In the Sigil project, open the file _content.opf_. Find the metadata section and erase it (including the opening and closing "metadata" tags) and replace what you just erased with the contents of the file _metadata.xml_ that you will find inside the _resources_ directory of this package.

### Finishing the Setup Process
Now edit the metadata (which after the prevoius step should have all the required fields) to reflect the information specific to the book that you are creating.

Oh --- and don't forget to save your work. You probably should have already saved it a number of times by now.

## Known Validators

There is [this one at eBookIt](https://www.ebookit.com/tools/bp/Bo/eBookIt/epub-validator).

The International Digital Publishing Forum has [a beta validator](http://validator.idpf.org/).
