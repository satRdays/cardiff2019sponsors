`cardiff2019poster.Rmd` is a template to create a poster based on elements from 
the Cardiff 2019 website. The stylesheets are generally imported from the 
same URLs as the website, apart from

 - The Bootstrap stylesheet. This was imported from 
 https://getbootstrap.com/docs/3.4/customize/ to remove print media styles 
 (and glyph icons) otherwise the fontawesome icons print as black circles.
 - The fontawesome stylesheet. Not sure why the Cardiff satRdays one didn't 
 work here.
 
The satRdays logo was chosen from https://github.com/satRdays/assets.

The HTML version was converted to PDF using 

    pagedown::chrome_print("cardiff2019poster.html")
    
The print style for Bootstrap means that the divs with the icons are printed 
in one column.

The PDF has a lot of white space and the fonts are generally too small. 
Therefore the PDF was scaled before printing to give a good enough result. 
To create flyers, `pdftk` was used to combine copies, so they could be printed 
4 to a page.

Probably better ways to go about this, but shared as a hacky solution that 
might be useful!