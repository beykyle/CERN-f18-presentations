
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

To contribute (if you are Dylan or Kyle):

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
 * Any other .sty file you care to include in your project
 * logos/ - A folder with the CERN logos used on the template
 * images/ - A folder with any images and figs to include

project directories
===

 * pres.tex - the actual presentation
 * makefile - this will handle compilation, and copy all necessary dependencies from include/ into the local folder. This is useful because anytime you update any dependencies in include, make will selectively copy the things you have updated.


Dependencies:
===
 * [TeXlive](http://www.tug.org/texlive/) 
 * [make](https://www.gnu.org/software/make/)
 
Building:
===
* Make the project in project directory p1/
```console
cd p1/
make
```

To delete all latex output and dependency copies in p1/
```console 
cd p1/
make clean
```
After doing this, you may have to make twice to reset the log and output files so that figures are set correctly.

To view the pdf output 
```console 
xdg-open p1/*.pdf 
```


