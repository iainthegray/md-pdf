# README

## How to do it

1. Install pandoc as normal
    `brew install pandoc`
1. Install [Prince](https://www.princexml.com/doc/installing/)
1. Do your markdown as normal. The notes below are some gotchas I have found with pandoc rendering and how to avoid them.
1. Copy the ea-doc.css file into a suitable directory, or indeed you can write your own css or edit this to your hearts content.
1. Run this pandoc command
   `pandoc -s --toc -c ea-doc.css upgrade.md -o upgrade.html`
1. Run this prince command to convert to pdf
    `prince upgrade.html -o upgrade.pdf`

Anything you dont like, you can edit the css to fit.

## Hacks
Cos I am lazy I have hacked some things together

* **Page Breaks** To put a page break in you need to add a horizontal rule in your md with 3 or more dashes with a blank line above and below


### Notes:
1. To get a sublist to render correctly, use 4 spaces to indent
1. To get an unordered list to render correctly - make sure that there is an empty line at the top of the list
1. When doing lists that have linebreaks in them but you want to continue the list then add a space line and indent the following lines until the next list point.

## Useful Links

How to do printing with css:
https://print-css.rocks/
