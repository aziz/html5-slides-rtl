# Style Documentation: #

put all the slides in an `article` tag inside a `section` tag with class `slides`.   
add a `rtl` class to section tag to make the slides right to left.  
In order to use custom persian font (Iranian Sans) just add the class `lang_fa` to the `html` tag.

## &lt;section class="slides"&gt; styles ##

### Layouts
* `layout-normal`: default layout, not needed. default slide size is 900x700
* `layout-widescreen`: makes slides 1100x700
* `layout-widescreen`: makes slides 1100x700 but the content width is just like normal (this increases padding on the left and right side of the slide)

### templates
* `template-default`:
* `template-io2011`:

## &lt;article&gt; styles ##

* `biglogo`:
* `nobackground`:
* `fill`:

## Slide Content Helpers: ##

* colors: `blue,yellow,green,red,black,white`
* `framed`: 
* `centered`:
* `noprettyprint`:
* `author`:
* `source`:
* `smaller`:
* `build`:

## Markup: #
h1: presentation title
h2: sub section
h3: slide title
p: normal text
ul,li,ol: bullet points
q: for qoutes
pre: for block of code
code: for inline code


* Style First Page: 

    article.biglogo {}

* Style each slide: select a name for your template and add it to the section tag
don't forget about the widescreen layout when styling your template

    .slides.template-your_template > article:not(.nobackground):not(.biglogo)
    .slides.layout-widescreen > article:not(.nobackground):not(.biglogo),
    .slides.layout-faux-widescreen > article:not(.nobackground):not(.biglogo)


# TODO #

* persian webfont
* touch styles in RTL

