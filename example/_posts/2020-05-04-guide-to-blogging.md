---
layout: post
title: Guide to Blogging with Jekyll
description: >
  A page showing Hydejack-specific markdown content.
image: 
  path: /assets/img/blog/example-content-iii.jpg
  srcset:
    1060w: /assets/img/blog/example-content-iii.jpg
    530w:  /assets/img/blog/example-content-iii@0,5x.jpg
    265w:  /assets/img/blog/example-content-iii@0,25x.jpg

# This overtakes sidebar image when post is opened
accent_image: 
  background: url('/assets/img/blog/jj-ying.jpg') center/cover
  overlay: false
accent_color: '#ccc'
theme_color: '#ccc'

# Set related posts to come at the bottom
related_posts:
  - example/_posts/2017-11-23-example-content-ii.md
  - /example/2012-02-07-example-content/
sitemap: false
invert_sidebar: true
---

This post contains Hydejack-specific markdown and HTML content.
{:.lead}

This makes a text bigger.
{:.lead}

Links can be doen the html way, like <a href="#">dis parturient montes</a>. "#" sends to the top of the page

Text can be **bold**, _italic_, or ~~strikethrough~~.

<!-- This enables table of contents -->
* toc
{:toc .large-only}

# Header 1

## Header 2

Here are some code block examples.

```js
// Javascript code with syntax highlighting.
var fun = function lang(l) {
  dateformat.i18n = require('./lang/' + l)
  return true;
}
```

```ruby
# Ruby code with syntax highlighting
GitHubPages::Dependencies.gems.each do |gem, version|
  s.add_dependency(gem, "= #{version}")
end
```

## Code Block Headers
Code blocks can now have headers:

~~~js
// file: 'hello-world.js'
console.log('Hello World!');
~~~

Headers are added by making the first line a comment of the form `(file|title): ['"].*['"]`, e.g.:

    ~~~js
    // file: 'hello-world.js'
    console.log('Hello World!');
    ~~~
    
Code blocks with and without headers now also come with a copy button. 
In the case of header-less code blocks, the button only shows on hover to prevent potential overlap.


### Header 3

> This is a blockquote following a header.
> blockquotes can be multiple lines

#### Header 4
*   This is an unordered list following a header.
*   This is an unordered list following a header.

##### Header 5
1.  This is an ordered list following a header.
2.  This is an ordered list following a header.

###### Header 6

How to make a small table.

| head1        | head two          | three |
|:-------------|:------------------|:------|
| ok           | good swedish fish | nice  |
| out of stock | good and plenty   | nice  |

### There's a horizontal rule below this.
* * *

### And a nested list:
- level 1 item
  - level 2 item
  - level 2 item
    - level 3 item

### Small image
![](https://assets-cdn.github.com/images/icons/emoji/octocat.png)

### Large image
![](https://guides.github.com/activities/hello-world/branching.png)

### Definition lists
Name
: Godzilla
Born
: 1952

Birthplace
: Japan

Color
: Green

- Abbreviations, like HTML should be defined like this `*[HTML]: HyperText Markup Language`.
- Citations, like <cite>&mdash; Mark otto</cite>, should use `<cite>`.
- ~~Deleted~~ text should use `~~deleted~~` and <ins>inserted</ins> text should use `<ins>`.
- Superscript <sup>text</sup> uses `<sup>` and subscript <sub>text</sub> uses `<sub>`.

Most of these elements are styled by browsers with few modifications on our part.

## Large Tables

| Default aligned |Left aligned| Center aligned  | Right aligned  | Default aligned |Left aligned| Center aligned  | Right aligned  | Default aligned |Left aligned| Center aligned  | Right aligned  | Default aligned |Left aligned| Center aligned  | Right aligned  |
|-----------------|:-----------|:---------------:|---------------:|-----------------|:-----------|:---------------:|---------------:|-----------------|:-----------|:---------------:|---------------:|-----------------|:-----------|:---------------:|---------------:|
| First body part |Second cell | Third cell      | fourth cell    | First body part |Second cell | Third cell      | fourth cell    | First body part |Second cell | Third cell      | fourth cell    | First body part |Second cell | Third cell      | fourth cell    |
| Second line     |foo         | **strong**      | baz            | Second line     |foo         | **strong**      | baz            | Second line     |foo         | **strong**      | baz            | Second line     |foo         | **strong**      | baz            |
| Third line      |quux        | baz             | bar            | Third line      |quux        | baz             | bar            | Third line      |quux        | baz             | bar            | Third line      |quux        | baz             | bar            |
| Second body     |            |                 |                | Second body     |            |                 |                | Second body     |            |                 |                | Second body     |            |                 |                |
| 2 line          |            |                 |                | 2 line          |            |                 |                | 2 line          |            |                 |                | 2 line          |            |                 |                |
| Footer row      |            |                 |                | Footer row      |            |                 |                | Footer row      |            |                 |                | Footer row      |            |                 |                |
{:.scroll-table}

## Math
Lorem ipsum $$ f(x) = x^2 $$.

$$
\begin{aligned}
  \phi(x,y) &= \phi \left(\sum_{i=1}^n x_ie_i, \sum_{j=1}^n y_je_j \right) \\[2em]
            &= \sum_{i=1}^n \sum_{j=1}^n x_i y_j \phi(e_i, e_j)            \\[2em]
            &= (x_1, \ldots, x_n)
               \left(\begin{array}{ccc}
                 \phi(e_1, e_1)  & \cdots & \phi(e_1, e_n) \\
                 \vdots          & \ddots & \vdots         \\
                 \phi(e_n, e_1)  & \cdots & \phi(e_n, e_n)
               \end{array}\right)
               \left(\begin{array}{c}
                 y_1    \\
                 \vdots \\
                 y_n
               \end{array}\right)
\end{aligned}
$$


## Message boxes
**NOTE**: You can add a message box.
{:.message}

![800x400](https://via.placeholder.com/800x400 "Large example image")

![400x200](https://via.placeholder.com/400x200 "Medium example image")

![200x200](https://via.placeholder.com/200x200 "Small example image")

## Large images
![Full-width image](https://via.placeholder.com/800x100){:.lead width="800" height="100"}

## Captions to images
![Full-width image](https://via.placeholder.com/800x100){:.lead width="800" height="100"}
A caption to an image.
{:.figure}

## Large quotes
> You can make a quote "pop out".
{:.lead}

## Faded text
I'm faded, faded, faded.
{:.faded}

[Modernized](#linking-in-style) [design](#whats-in-the-cards), [big headlines](#ready-for-the-big-screen), big new features: [Built-In Search](#built-in-search), [Sticky Table of Contents](#sticky-table-of-contents), and [Auto-Hiding Navbar](#auto-hiding-navbar). That [and more](#and-much-more) is Hydejack 9.

- Table of Contents
{:toc .large-only}

## Linking in Style

 With Hydejack 9, the [link style](#linking-in-style) has been revamped so that legibility is no longer tied to the choice of accent_color, giving you much more freedom in creating a unique design flavor for your site.
 
## Ready for the Big Screen

With version 9, Hydejack takes full advantage of large displays. Whether it's design indulgences such as oversized headlines, or quality of life improvements such as a floating table of contents, Hydejack now finds use for all that extra screen real estate[^1]. 
 
## What's in the Cards?

Good images are key to making the most out of content cards. For that reason, a [chapter on images](../../docs/basics.md#adding-images) has been added to the documentation.
 
## Built-In Search

Hydejack now has Built-In Search. It even works offline. I've been prototyping many approaches and eventually settled on a fully client-side, off-the-main thread solution that perfectly fits the use case of personal sites and shows surprisingly good results[^2]. 
 
## Auto-Hiding Navbar

A navbar that's there when you need it, and disappears when you don't. Simple as that.
 
## Sticky Table of Contents

Already a staple on so many sites on the web, this pattern is now also available in Hydejack. 
What's unique about it is that it simply picks up the table of contents already created by kramdown's `{:toc}` tag and transparently upgrades it to a fully dynamic version.
 
## …and much more

Other noteworthy changes include:
- Support for Jekyll 4
- Choice between MathJax and KaTeX for math rendering
- Use of `jekyll-include-cache` for drastically improved page building speeds
- New variables configuration file — adjust content width, sidebar width, font size, etc...
- ...and the option to disable grouping projects by year.

Read the the [CHANGELOG](../../CHANGELOG.md){:.heading.flip-title} for the full scope of features and improvements made in Hydejack 9.
Maybe just glance at it to confirm that it is indeed a pretty long list.
 

<div class="gumroad-product-embed" data-gumroad-product-id="nuOluY"><a href="https://gumroad.com/l/nuOluY">Loading…</a></div>


# New in Hydejack 9.1

## Inverted Sidebars
The colors on the sidebar can now be inverted to allow brighter sidebar images. This can be enabled per-page in the front matter:

```yml
invert_sidebar: true
```

## Stripe-ified Design
Most elements now have rounded borders, making the design look more modern (dare I say "Stripe-ified") than ever before. 

The goal of Hydejack was always to provide a theme that looks "designed" combined the amenities of a typical Jekyll theme for coders.
This is an important step in maintaining this goal.

At the same time, I'm introducing nerdy elements like [breadcrumbs](#serp-breadcrumbs), that are almost ornamental in nature.
You wouldn't find these on other Stripe-like designs, but I think they are appealing to developer types like myself. 
Like most additions to Hydejack, they can be disabled via configuration. 

## Resume Download Buttons
Resumes can now have download buttons:

![Download Buttons](/assets/img/blog/9.1.0-3.png){:.border.lead width="1776" height="258" loading="lazy"}

Resumes can now have download buttons.
{:.figcaption}

The documentation has been updated with a chapter on [how to configure the buttons](/docs/basics/#downloads).


## SERP Breadcrumbs
Added breadcrumbs above page title:

![Breadcrumbs](/assets/img/blog/9.1.0-2.png){:.border.lead width="1588" height="164" loading="lazy"}

Bread crumbs are now shown above each page title.
{:.figcaption}

Note that this requires a [directory-like URL structure](https://qwtel.com/posts/software/urls-are-directories/) on your entire site, 
otherwise the intermediate links will point to nonexisting sites.

On a side note, Hydejack now has built-in tooltips for abbreviations like SERP (activated via tap/click).
See [Example Content](/blog/hyde/2012-02-07-example-content/#inline-html-elements) on how to add them to your content.


## Last Modified At
Blog posts can now have a "last modified at" date in the sub title row.

![Last modified at](/assets/img/blog/9.1.0-1.png){:.border.lead width="1254" height="218" loading="lazy"}

Note that this depends on the `last_modified_at` property of the page, which must be either set manually in the frontmatter (not recommended), or via a plugin like [`jekyll-last-modified-at`](https://github.com/gjtorikian/jekyll-last-modified-at). Note that the later is not available when building on GitHub Pages and can increase build times.


## Clap Button Preview
I've been trying something new with [**getclaps.app**](https://getclaps.app/), a feedback and analytics tool for personal sites like those powered by Hydejack. 

<!-- <clap-button style="--clap-button-color:var(--body-color);margin:2rem auto 3rem;width:3rem;height:3rem;font-size:smaller" nowave></clap-button> -->

It is a separate product from Hydejack and not enabled by default. Because it depends on a backend component, it requires a monthly fee. 
If enabled, it is placed below posts and pages where the dingbat character (❖) used to be.

I can't claim that this product is fully baked (feedback welcome), but I've been using it on my personal site and here for the last couple of months with no issues.
For more, see [the dedicated website](https://getclaps.app/).

***
{:style="margin:2rem 0"}

There are many more changes and bugfixes in 9.1. See the [CHANGELOG](/changelog/){:.heading.flip-title} for details.


## Credits

<span>Photo by <a href="https://unsplash.com/@jjying?utm_source=unsplash&amp;utm_medium=referral&amp;utm_content=creditCopyText">JJ Ying</a> on <a href="https://unsplash.com/?utm_source=unsplash&amp;utm_medium=referral&amp;utm_content=creditCopyText">Unsplash</a></span>

*[SERP]: Search Engine Results Page



[^1]: If you are a fan of the old two-column layout, or don't like modern design tropes such as mega headlines, Hydejack lets you revert these changes on a case-by-case basis via configuration options.

[^2]:
      Search was mainly tested for English and German. Please let me know about issues in other languages. 
      While I've tried to find a multi-language solution, most showed drastically worse  results for the English base case.
      If you're technically inclined, you can adopt the code located in `_includes/js/search-worker.js` to your needs.

*[HTML]: HyperText Markup Language
*[CSS]: Cascading Style Sheets
*[JS]: JavaScript
[mm]: https://guides.github.com/features/mastering-markdown/
[ksyn]: https://kramdown.gettalong.org/syntax.html
[ksyntab]:https://kramdown.gettalong.org/syntax.html#tables
[ksynmath]: https://kramdown.gettalong.org/syntax.html#math-blocks
[katex]: https://khan.github.io/KaTeX/
[rtable]: https://dbushell.com/2016/03/04/css-only-responsive-tables/
