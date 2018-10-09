
Based on https://github.com/icot/cern-beamer:

A [Beamer](https://bitbucket.org/rivanvx/beamer/wiki/Home) template mimicking
the official [CERN](www.cern.ch) template for presentations as shown
[here](http://design-guidelines.web.cern.ch/presentations).

[CERN](www.cern.ch) is the source of the images used as ghaphic resources for
this theme, and retains the sole copyright of all related imagery.
For more information regarding this, please take a look to their
[copyright](http://cern.ch/copyright).

CERN-f18-presentations
===========

These directories contain the LaTeX source for Kyle Beyer and Dylan Hatch's presentations for the ITK Strips DAQ 
project, on the ATLAS experiment. All work took place at CERN during the fall of 2018, for the University of Michigan REU semester abroad program, sponsored by the Lonsberry foundation.

Contributing
===

To contribute:

```console 
git clone https://github.com/beykyle/CERN-f18-presentations.git
git checkout -b myname 
```

Edit files and commit as desired in your branch. 

```console
git push --set-upstream myname
```

Then create a pull request to master


Structure
====

 * The top level directories correspond to a presentation, or the general include directory
 * Each presentation goes in a new directory, named p1 through pn
 * General include files go in include/ 


include directory
=====

 * beamerthemeCERN.sty - The beamer theme definition (colors, fonts, etc)
 * logos/ - A folder with the CERN logos used on the template
 * images/ - A folder with images and figs to include

project directories
===

 * pres.tex - the actual presentation


Building with Latexmk
===
