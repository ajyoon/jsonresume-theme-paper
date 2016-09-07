# JSON-Resume-Paper
## (With customizations by Andrew Yoon)

This is a theme for [JSON Resume](http://jsonresume.org/).
This is a fork of the `jsonresume-theme-paper` theme by Tim Daub
with minor customizations I made for my own resume.

The original git branch can be found on Github
[here](https://github.com/TimDaub/jsonresume-theme-paper).

## Demo
An example of this theme with its customizations can be found
on my website [here](http://andrewjyoon.com/static/resume.html).

## Installation
To get set up, clone this repository to your local system and
install its dependencies with NPM:

    git clone git@github.com:ajyoon/jsonresume-theme-paper.git
    cd jsonresume-theme-paper
    npm install

While any of the JSON Resume theme supporting build tools should
work, this has only been extensively tested using
[hackmyresume](http://please.hackmyresume.com/) for HTML output
and [wkhtmltopdf](http://wkhtmltopdf.org/downloads.html) for PDF
rendering. 

You can install `hackmyresume` with NPM:

    npm install hackmyresume [-g]

To install `wkhtmltopdf` visit their website
[here](http://wkhtmltopdf.org/downloads.html). Be sure to install
the latest stable version for proper PDF support.

## Use
Once everything is installed, you can build your JSON resume like so:

    cd /path/where/my/json/resume/is
    hackmyresume BUILD my_resume.json TO my_resume.html \
        -t /path/to/jsonresume-theme-paper/
    # And export to PDF
    wkhtmltopdf --print-media-type -s Letter resume.html resume.pdf

## License
Available under [the MIT license](http://mths.be/mit).
