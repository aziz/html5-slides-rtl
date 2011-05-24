### [RTL Demo](http://aziz.github.com/html5-slides-rtl/index_rtl.html) and [English Demo](http://aziz.github.com/html5-slides-rtl/) #

![html5slides with RTL support](http://f.cl.ly/items/0D0n2a2L1s0E3O432z2Z/html5slides_rtl_fa.jpg)

# Documentation: #
Put all the slides in an `article` tag inside a `section` tag with class `slides` (look at the templates for the markup).
Add a `rtl` class to section tag to make the slides right to left. In order to use custom persian font (Iranian Sans) add the class `lang_fa` to the `html` tag.

## &lt;section class="slides"&gt; styles ##

### Layouts
* `layout-normal`: default layout, not needed. default slide size is 900x700
* `layout-widescreen`: makes slides 1100x700
* `layout-widescreen`: makes slides 1100x700 but the content width is just like normal (this increases padding on the left and right side of the slide)

### templates
* `template-default`
* `template-io2011`

### direction ###
* `rtl`

## &lt;article&gt; styles ##

* `biglogo`: The first slide where you put your logo, the presentation title and your name will come on the second slide
* `nobackground`: Clean slate slide
* `fill`: Where you have an image in the slide which you want it to fill the whole slide and work as a background image

## Slide Content Helpers: ##

* `blue,yellow,green,red,black,white`
* `centered`
* `framed`: put a box around your content
* `noprettyprint`: adding this tag to `pre` tag will disable the syntax highlighting on it
* `author`: used with `q` tag in quote slides
* `source`: add a source to the bottom of your slide
* `smaller`: make the font of the whole slide a little smaller
* `build`:

## Markup: #
* `h1`: presentation title
* `h2`: sub section
* `h3`: slide title
* `p`: normal text
* `ul,li,ol`: bullet points
* `q`: for qoutes
* `pre`: for block of code
* `code`: for inline code


## Makeing your own template ##



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

