## News

- 22/06/2015 changes moved from README.md to CHANGELOG.md

- 18/06/2015 replaced `--mathml` option with `--mode`. For `mathml` support, use`mathml` option for `tex4ht.sty`.

  - lot of stuff was fixed in `epub3` support. 
  - new command `\OpfAddProperty`  

- 14/01/2015 thanks Volker Gottwald for guide on [installing and using 
  tex4ebook](https://d800fotos.wordpress.com/2015/01/19/create-e-books-from-latex-tex-files-ebook-aus-latex-tex-dateien-erstellen/)  on Windows

- 23/11/2014 added new command `\OpfGuide`, for adding items to `<guide>`
  section in the `opf` file. This is useful for `epub` and `mobi` formats.
  Usage:

        \OpfGuide[filename]{title}{reference type}

  `filename` is optional, current file name is used when empty. See 
  [epub secrets](http://epubsecrets.com/where-do-you-start-an-epub-and-what-is-the-guide-section-of-the-opf-file.php)
  article

- 20/10/2014 fixed issues with starred sections

  - files created by starred sectioning commands (`\chapter*`, `\section*`)
    should be included in normal reading order now

- 16/09/2014 new features added

  - new configuration file for `--tidy` option, mathml and html5 elements are 
    supported. This means that many validation errors in `mathml` output
    can be fixed with `--tidy` option
  - added configuration for all languages supported by `babel`
  - `woff` and `ttf` fonts are supported
  - added inline footlines in `epub3` format
  - added `no-cut` command line option for breaking sections and chapters into
    standalone pages



- Please support [iniciative for improving mathml
  support](http://www.ulule.com/mathematics-ebooks/) in Gecko and Webkit
  engines. This will hopefully improve also Epub3 readers.

  

- 10/08/2013
  [`make4ht`](https://github.com/michal-h21/make4ht) is now standalone
  application which `tex4ebook` depends on. You must 
  [install   it](https://github.com/michal-h21/make4ht#instalation) in order to
  use current `tex4ebook` version.