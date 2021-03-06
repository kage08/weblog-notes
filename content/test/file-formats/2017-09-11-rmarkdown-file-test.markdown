---
title: ".Rmarkdown File Test"
author: Peter Baumgartner
date: '2017-09-11'
slug: rmarkdown-file-extension
draft: yes
description: What are the properties of the `.Rmarkdown` extension in relation to
  `Rmd` and `md` files?
---


## Advantages of using `.Rmarkdown` files

+ This file type is able to run R code snippets like `.Rmd` files. Numbered tables, figures, equations, and theorems are also supported.
+ But `.Rmarkdown` files compiles not to `.html` but to '.markdown' files, which are easier to read. This is particulary important when reviewing [GitHub](https://github.com/) pull requests.

You can use the `back apostroph` or the <code>code command</code> for red flagged text. But better use always the code command.

## Diadvantages of using `.Rmarkdown` files

* It uses Hugo `Blackfriday` und not `Pandoc` as rendering machine. Consequently you cannot use the much richer set of `Pandoc` converter such as citations. 

    + Math expressions only work if you have installed the `xaringan` package and applied the JavaScript solution mentioned in [Section A.3 of the blogdown book](https://bookdown.org/yihui/blogdown/javascript.html).
        
    + You cannot directly use Markdown syntax in table or figure captions, but you can use text references as a workaround (see bookdown’s documentation).
        
  * HTML widgets are not supported.
  * RStudio snippets are not supported


{{% notice note %}}
There is an issue with nested bullet lists with Blackfriday<br />
Use 4-spaces rather than 2-space indentations.<br />
Tab work again only when it defaults to 4 spaces.
{{% /notice %}}

## Detailed comparison is necessary

One has to inspect the differences detailed. 

* See the possiblities and options for Hugo [Blackfriday](https://gohugo.io/content-management/formats/) or look into in the [GitHub pages of the Blackfriday project](https://github.com/russross/blackfriday).

* See the funtionality of [Pandoc](http://pandoc.org/) processor



### Test with an R code snippet

```r
2 + 2
```

```
## [1] 4
```

