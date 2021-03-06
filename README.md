UW-WKRPT
--------

Thanks for downloading uw-wkrpt.  This is a LaTeX document class that I
developed to make you life easier, when writing work term reports for
the University of Waterloo.

If you do not know LaTeX, please learn!  It is not too
difficult to use, and is really quite helpful.  You can read the
workreport-sample.pdf file included in this tarball, as well as
the following two books:

A simplified introduction to LaTeX
  http://carbon.cuderwer.edu/~hgreenbe/aboutme/simplified-intro.html

A not so short introduction to LaTeX2e: or LaTeX2e in 113 minutes
  http://people.ee.ethz.ch/~oetiker/lshort/

You can also find more information on-line.  There is a FAQ
at: http://faq.tug.org and an page listing documentation for beginners
at: http://www.tug.org/begin.html

Please send me any comments, bug reports, bug fixes and 
suggestions that you may have.  You can get the newest copy of this
document class from my school-hosted website at:
  http://www.eng.uwaterloo.ca/~sfllaw/programs/uw-wkrpt/


FILES
-----

There are several files in this tarball.  

* The README file is the one you are reading now.

* The NEWS file is a list of interesting things that have changed
  since the last release.

* The INSTALL file tells you how to install and use this document 
  class.

* The ChangeLog file is a record of the changes made to the software.

* COPYING contains a copy of the GNU General Public License.

* uw-wkrpt.ins is the docstrip installer.  Please see the INSTALL file.

* uw-wkrpt.dtx is the docstrip document that contains the entire
  uw-wkrpt package.

* uw-wkrpt-\*.tex are example documents written using uw-wkrpt.cls.  
  It illustrates the way to write a document, and tries to adhere as 
  closely to the guidelines as possible.

* uw-wkrpt.bib is the bibliography or references list that is imported 
  by the example reports.

* don-hires.pdf is a picture of Donald E. Knuth, acquired from his 
  website and used in workreport-sample.tex.

OTHER USEFUL PACKAGES
---------------------

You may wish to load some other useful packages to make your life
simpler, and your work report nicer.  After the ``\documentclass{uw-wkrpt}''
line, just add ``\usepackage{foo}'', where ``foo'' is the package name.

* acronym
    for spelling out acronyms in full, the first time only.

* longtable
    for tabular environments that break pages.

* tabularx
    for tabular environments that know how wide they are.

* ltxtable
    for a merge of longtable and tabularx, which may not work.

* times, mathptm
    For using the Times font in your text and math.

-- Simon Law <sfllaw@uwaterloo.ca>  Wed, 30 Apr 2003 19:34:41 -0400


# Instructions for MAC users

Big thanks to Val (vtsatskin) for these instructions for all you mac users out there that
want to use this template!

## Install MacTex

LaTeX is distributed on Mac OS X via MacTex. As of this wriiting the installer is 2.3 GB. It's pretty large so it'll take some time to download.

You can find the latest version on [their website](https://www.tug.org/mactex/).

## (Optional) Add /usr/texbin to your PATH

You can skip this section if you don't use a different system shell (i.e. you use bash).

If you're using a shell other than bash, you'll want to add /usr/texbin to your PATH.

### zsh configuration

Open `~/.zshrc` in your favorite editor and find a line similiar to:

    export PATH="$HOME/bin:/usr/local/bin:/usr/bin:/bin:/usr/sbin:/sbin"

You'll want to add `/usr/texbin` to the path like so (it's at the end):

    export PATH="$HOME/bin:/usr/local/bin:/usr/bin:/bin:/usr/sbin:/sbin:/usr/texbin"

## Generating PDFs

1. In Terminal.app, `cd` into your work report directory
2. Run `make`. You'll see a bunch of messages scroll across your terminal.
3. Run `open Default_Report.pdf` to open the generated PDF.

Every time you make a change to the LaTeX, you'll want to run `make` again to see your changes. Steps 2 and 3 can be combined into one command such as `make && open Default_Report.pdf`
