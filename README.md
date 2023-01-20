medium-act-iii-book
# Book of Act III on Medium

# Welcome
This is an Asciidoc book of Creations's "ACT III". It simply takes all their [medium posts](https://medium.com/act-i) and joins them together for ease of reading.  The intention is to be entirely faithful to the original posts - I've not even fixed the few spelling mistakes - while allowing various output versions to be generated, e.g. HTML, and .mobi for Kindle e-readers.  It is made available under the same Creative Commons Attribution-ShareAlike-4.0-International licence as the original posts. 

# Downloads
If you want the PDF, or MOBI versions of this book, click on the "releases" tab above.

# Generating the book yourself
All these generators require you to have installed [asciidoctor](https://asciidoctor.org/docs/user-manual/). Then select the command you require to generate the output you desire.

## HTML 
To generate the HTML version of this book, run the following command in the base directory of this repository:

    asciidoctor medium-act-iii-book.adoc

## PDF
To generate the PDF version of this book, you additionally need to install [asciidoctor-pdf](https://asciidoctor.cn/docs/convert-asciidoc-to-pdf/) with the following command:

    gem install --pre asciidoctor-pdf

Then you can run the following command in the base directory of this repository:

    asciidoctor-pdf medium-act-iii-book.adoc

## .KPF (Kindle)
KindleGen is no longer available for download. Please use Kindle Previewer to convert, preview, and validate your eBooks. Kindle Previewer provides the same functionality of KindleGen and, in addition, provides:

- Latest Kindle Conversion software that provides up-to-date validation for Enhanced Typesetting books (currently available for books in all languages except Simplified Chinese, Japanese, and Russian).
- Choice of using in Graphical User Interface (GUI) for a visual inspection of your book, or, Command Line Interface (CLI) mode for bulk validation.
- Faster preview and validation with features like thumbnails, auto-previews, and filters for pages with images, tables, drop caps, and links.

We recommend using EPUB format for publishing new reflowable titles and updating previously published titles. MOBI should only be used when testing on older devices that do not support Enhanced Typesetting.

[Click here to visit the Kindle Previewer product page](https://tinyurl.com/y84exbka?rw_useCurrentProtocol=1&ref_=amb_link_n94Zbz6DNuSumTne6o22Bg_1)

# Contributing
Contributions are cool, and also very welcome.  There is a [code of conduct](CODE_OF_CONDUCT.md), and a [contribution guide](CONTRIBUTING.md) which you can familiarise yourself with if you want to get involved (even if its just fixing a typo).  They should be _very_ unsurprising to anyone used to the OSS world.

# To Do
* Fix xref rendering on .mobi (Kindle) file generation - it doesn't work
* Replace the formulae image in chapter 19 with the latex equivalent (https://github.com/asciidoctor/asciidoctor-latex)
* Change the type-setting so that paragraphs in the ```.mobi``` output aren't indented
* Add a Travis build
