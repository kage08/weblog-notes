---
title: excerpt-include
author: Peter Baumgartner
date: '2019-06-05'
description: It displays ‘excerpted’ (that is, a segment of) content from one page
  into another.
disable_comments: yes
draft: yes
---

The Excerpt Include shortcode is used to display 'excerpted' (that is, a segment of) content from one page in another.
Before you can use this shortcode, the excerpt must have been defined using the Excerpt shortcode. {{%alert info%}}Note that you can have more than one Excerpt Include shortcode on a page (although you can have only one Excerpt shortcode on a page).{{%/alert%}}


## Usage

| Parameter | Default | Description |
|:--|:--|:--|
| filename | **required** | Type the filename of the page that contains the excerpt to be displayed.<br/>Path is relative to the content folder|
| panel | none | Determines whether docDock will display a panel around the excerpted content. The panel includes the given panel's value and the border of the panel. By default, the panel and title are not shown.|

## Demo
The paragraph below shows an example of an Excerpt Include shortcode, containing content from an excerpt which we have defined on the Excerpt shortcode page. On the Excerpt Include shortcode below, we have set the options to show both the title of the page and the panel surrounding the content.

	{{%/*excerpt-include filename="shortcodes/excerpt.md" panel="From excerpt page" /*/%}}

{{%excerpt-include filename="archive/shortcodes/excerpt.md" panel="From excerpt page" /%}}
