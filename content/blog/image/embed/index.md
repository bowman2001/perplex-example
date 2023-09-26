---
authors: [Georg Makowski]
title: Embedded image (float)
description: Layout options for inline images
subtitle: false
date: 2023-03-23T10:10:51+01:00 
categories: [markdown]
tags: [image, block]
series: [images]
---

This page demonstrates the layout for advanced embedded images.
{.p-first}
<!--more-->

For the Markdown syntax see [basic image](https://perplex.desider.at/doc/basic/image) and [enhanced image](https://perplex.desider.at/doc/improved/image/syntax).

## At the beginning

### Small width (default)

![](small-portrait) {{% pangram 15 %}}
{.placeholder data-pagefind-ignore="all"}

![](small.yaml?posh=right) {{% pangram 15 %}}
{.placeholder data-pagefind-ignore="all"}

### Tiny width

![](tiny-portrait.yaml) {{% pangram 13 %}}
{.placeholder data-pagefind-ignore="all"}

![](tiny.yaml?ph=right) {{% pangram 13 %}}
{.placeholder data-pagefind-ignore="all"}

### Micro size

![](micro) {{% pangram 9 %}}
{.placeholder data-pagefind-ignore="all"} 

![](micro?ph=right) {{% pangram 9 %}}
{.placeholder data-pagefind-ignore="all"}

## In the middle of a text block

Images with the default small width need some additional spacing when they are placed in the middle of a text block:

{{% pangram 4 %}} ![](small?pv=middle) {{% pangram 6 %}}
{.placeholder data-pagefind-ignore="all"}

{{% pangram 8 %}}
{.placeholder data-pagefind-ignore="all"}

{{% pangram 4 %}} ![](small?ph=right&pv=middle) {{% pangram 6 %}}
{.placeholder data-pagefind-ignore="all"}

{{% pangram 8 %}}
{.placeholder data-pagefind-ignore="all"}

## In lists

Embedded images always scale to a fixed percentage of the containing text width.

### Micro width

1. ![](micro) {{% pangram 4 %}}

   - ![](micro?posh=right) {{% pangram 4 %}}

   - ![](micro) {{% pangram 4 %}}

2. {{% pangram 2 %}} ![](micro?posh=right) {{% pangram 3 %}}
{.placeholder data-pagefind-ignore="all"}

### Tiny width

1. ![](tiny.yaml) {{% pangram 7 %}}

   - ![](tiny.yaml?posh=right) {{% pangram 7 %}}

   - ![](tiny.yaml) {{% pangram 7 %}}

2. {{% pangram 4 %}} ![](tiny.yaml?posh=right&posv=middle) {{% pangram 5 %}}
{.placeholder data-pagefind-ignore="all"}

### Variable text width

Because stand-alone images do not fit in lists or other structured text blocks, we need embedded ones to fill up the full width of the containing text block.

#### Normal list

1. {{% pangram 2 %}} ![](textvar)

2. {{% pangram 2 %}} ![](textvar)
{.placeholder data-pagefind-ignore="all"}

#### Columned list

1. {{% pangram 1 %}} ![](textvar)

2. {{% pangram 1 %}} ![](textvar)
{.col2 .placeholder data-pagefind-ignore="all"}

#### Loose definition list

First term
: {{% pangram 3 %}} ![](textvar)

Second term
: {{% pangram 3 %}} ![](textvar)
{.dl-loose .placeholder data-pagefind-ignore="all"}
