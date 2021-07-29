# Presentations: An HTML Presentation Framework

Forked from [dzslides](https://github.com/paulrouget/dzslides), this is a framework for building presentations in HTML. Right now, it's pretty barebones.

## Instructions

- Clone this repo.
- duplicate `template.html` and rename it to whatever you want. 
- Start writing out your slides! Put each slide into it's own `<section>` block. For more style examples, check out the `example.html` slide or read the minimal documentation below.
- If you want to see your changes update live as you save them, make sure you have node installed, run `npm install` and use `npm run dev` to start a development server.

## Documentation

### Section
a `section` block wraps your code into a slide. Sections are center aligned by default.

### Column Layout
Use the class `.columns` on a section to indicate a column layout slide. Within `.columns`, you can use `.two-col` to indicate a 50% width column, or `.three-col` to indicate a column that takes up a third of the screen.

Column height is set to auto and centered vertically. To take up the full height, add a class of `.tall` to your `.tw-col` or `.three-col` div.

You can even embed layouts, check out `example.html`.

### Titles

`h1` to `h4` are center aligned titles with varying font-weights. 

### Body Text
the `<p>` blocks are left-aligned, but vertically centered. To center align your text, use the `.center` class. By default the text blocks take up 60% of the width. For a longer text block, use `.fw` on your `<p>` block. This stands for _full-width_, not _f*ck with_. 

To use a `<p>` block as a subtitle to an H1, add the `.subtitle` class.

For smaller text, you can use `.small`, which reduces the size and changes the color a little bit.


### Background Image / Video Slides

To have an image take up the full width and height of a slide, you can place your `<img>` or `<video>` in a `<figure>` block. If you want to have text overlaid on the video/image, use a `<figcaption>` block. To blur the image or video, add the `.blur` class to your asset.

## Extending

Edit the CSS file `assets/userstyles.css` to change up the colors or fonts to your hearts desire. I wouldn't mess with `assets/defaultstyle.css` because that's the default slides from **dzslides**, but if you know what you're doing, go right ahead.

## TODO 

- [x] Add a live-reload server
- [  ] Export to pdf, using puppeteer or something.
- [  ] Markdown _to_ HTML _to_ PDF, probably using pandoc.
- [  ] Probably blog about this, because my blog is looking bare af.
- [  ] Theme support. If I wanna go overkill I can try to figure out Pywal integration.

## License

                DO WHAT THE EFF YOU WANT TO PUBLIC LICENSE
                        Version 2, December 2004

    Everyone is permitted to copy and distribute verbatim or modified
    copies of this license document, and changing it is allowed as long
    as the name is changed.

                DO WHAT THE EFF YOU WANT TO PUBLIC LICENSE
      TERMS AND CONDITIONS FOR COPYING, DISTRIBUTION AND MODIFICATION

    0. You just DO WHAT THE EFF YOU WANT TO.
