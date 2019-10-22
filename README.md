
 svg and svg-extract -- Include and extract SVG pictures in LaTeX documents 
----------------------------------------------------------------------------

 Copyright (C) Philip Ilten <philten@cern.ch>, 2012-2016  
 Copyright (C) Falk Hanisch <hanisch.latex@outlook.com>, 2017-

 svg 2019/10/10 v2.02c

----------------------------------------------------------------------------

 This material is subject to the LaTeX Project Public License version 1.3c 
 or later. See http://www.latex-project.org/lppl.txt for details.

----------------------------------------------------------------------------


Summary
-------

The **svg** package is intended for the automated integration of SVG graphics 
into LaTeX documents. Therefor the capabilities provided by ***Inkscape***---or 
more precisely its command line tool---are used to export the text within a SVG 
graphic to a separate file, which is then rendered by LaTeX. For this purpose 
the two commands `\includesvg` and `\includeinkscape` are provided which are 
very similar to the `\includegraphics` command of the **graphicx** package.

In addition, the package **svg-extract** allows the extraction of these 
graphics into independent files in different graphic formats, exactly as 
it is rendered within the LaTeX document using either ***ImageMagick*** or 
***Ghostscript***


Versions
--------

**v2.02d** (2019/10/22)
+ fix bugs with current kernel (2019/10/01) regarding file name parsing

**v2.02c** (2019/10/10)
+ fix bugs with current kernel (2019/10/01) regarding file name parsing

**v2.02b** (2018/11/12)
+ fix bug for package **tikzscale** which changes `includgraphics` globally

**v2.02a** (2018/10/17)
+ fix bug for package **polyglossia** which fakes **babel** poorly

**v2.02** (2018/09/08)
+ distortion of included and extracted graphics supported with options `distort` 
  (or `keepaspectratio`) and `extractdistort` as well as rotation for 
  extractions (`extractangle`)
+ fixed errors with active double qoutes from **babel** in path arguments
+ multiple dots within file names possible
+ package **trimspaces** required

**v2.01** (2017/11/29)
+ new option `svgextension` to change the format of files exported by
  ***Inkscape*** from `svg` to a custom one
+ usage of `\input{tex filename}` within ***Inkscape*** graphics
  locates files in all declared searched folders

**v2.00b** (2017/05/23)
+ improved warnings, if package **svg** is loaded by package **svg-extract**

**v2.00a** (2017/03/28)
+ Bug fix for checking stock- and mediasizes

**v2.00** (2017/03/27)
+ New maintainer: Falk Hanisch
+ Re-implementation from scratch
+ functionality split in two packages **svg** and **svg-extract**
+ package **svg** intended for including SVG files
+ package **svg-extract** for extracting graphic files rendered with LaTeX
+ **svg-extract**: enhanced support for ***ImageMagick***
+ **svg-extract**: support for ***Ghostscript*** added
+ package **subfig** not required anymore
+ support of subfigures stopped due to the huge number of packages which deal 
  with this topic and the large variety of implementing this functionality; 
  naming exported graphics after their consecutive numbering can't be ensured
  for all variants of subfigures, so it's neglected

**v1.0** (2016/10/10)
+ initial version by Philip Ilten
