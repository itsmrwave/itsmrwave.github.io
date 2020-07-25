---
layout: page
title: Colophon
permalink: /about/colophon/
sitemap: true
---

Traditionally, [colophons][definition-colophon] were a publisher's emblem or
imprint to give information about its authorship and printing. Instead, here I
describe the **ideas, tooling, and organization behind this creative work**. You
can learn more about the purpose and content of this website, as well as the
author ... [elsewhere][site-pages-about].

### Design & Imagery 🎨

The site layout is powered by [Foundation 5][foundation-v5], primarily to take
advantage of it's [responsive grid system][foundation-v5-grid]. All the styling
on top of that is my own _creative expression_ of a _timeless_ and
_minimalistic_ design.

The [favicon (the little crown)][favicon] is derived from [my logo (encircled
crown)][logo] was [designed by me][logo-design]. I love colour and the [shifting
chameleon colours on this site][shifting-colours] provided a fun way for me to
incorporate that into my design while maintaining minimalism.

### Tech & Tools 🛠️

The entire website is a static website that is generated by [Jekyll][jekyll].
Hosting is via [GitHub Pages][github-pages] which in turn is configured with
[this GitHub repository][github-website-repository]. I just edit, commit the
changes, push, and my changes are live!

The [sitemap][sitemap] and feeds for the [articles & thoughts][feed-articles],
[blog][feed-blog] and [code minutae][feed-minutae] sections are all [generated
using Jekyll’s Liquid templates][feeds-source-code].

All the feeds are [Atom 1.0 feeds][atom-feed-standard]. I don't use [the
`jekyll-feed` plugin][jekyll-feed], because it didn't exist at the time I
created this site. Also because of the way I've chosen to structure my site into
different segments (more on this below).

JavaScript is kept to a minimum on this site, however I've used a few small
libraries here and there (mostly for fun). I use:

* [Highlight.js][js-highlight] to format code blocks where I share code.
* [Modernizr.js][js-modernizr] for all its shims, fallbacks, and polyfills in
  order to implant HTML5 functionality in browsers that don't natively support it.
* [NProgress.js][js-nprogress] to provide realistic trickle animations on page
  load.
* [Turbolinks.js (Classic)][js-turbolinks-classic] to provide some speedup from
  not having to download or parse the CSS & JS files on every page load.

On the styling front, I have:

* [FontAwesome.css][css-fontawesome] which is a icon library + toolkit.
* [Normalize.css][css-normalize] to makes browsers render all elements more
  consistently and in line with modern standards.

My current preferred code editor is [VSCode][vscode]. It's free plus there are
tonnes of extensions such as the [markdownlint extension][vscode-markdownlint]
which really comes in handy while working on this site.

### Structure & Breakdown 🗄️

This site has it's own unique structure. I'll break it down to you below:

* [Articles & Thoughts][site-articles] – short snippets of smart ideas that I
  came across on the Internet (title of the post usually links back to the
  source).
* [Blog][site-blog] – long form posts which comprise of my own writing.
* [Code Minutae][site-minutae] – snippets of code that I thought of sharing.
* Pages – standalone pages that don't fit any of the above categories such as
  [this page][site-pages-colophon] and [the about page][site-pages-about].

[atom-feed-standard]: https://en.wikipedia.org/wiki/Atom_(Web_standard)
[css-fontawesome]: https://fontawesome.com
[css-normalize]: https://necolas.github.io/normalize.css/
[definition-colophon]: https://www.lexico.com/en/definition/colophon
[favicon]: /favicon.ico
[feed-articles]: /feeds/articles.xml
[feed-blog]: /feeds/blog.xml
[feed-minutae]: /feeds/minutae.xml
[feeds-source-code]: https://github.com/itskingori/itskingori.github.io/blob/master/_layouts/atom.html
[foundation-v5-grid]: https://get.foundation/sites/docs-v5/components/grid.html
[foundation-v5]: https://get.foundation/sites/docs-v5/
[github-pages]: https://pages.github.com
[github-website-repository]: https://github.com/itskingori/itskingori.github.io
[jekyll-feed]: https://github.com/jekyll/jekyll-feed
[jekyll]: https://jekyllrb.com
[js-highlight]: https://highlightjs.org
[js-modernizr]: https://modernizr.com/
[js-nprogress]: http://ricostacruz.com/nprogress/
[js-turbolinks-classic]: https://github.com/turbolinks/turbolinks-classic
[logo-design]: /blog/2013/04/logo/
[logo]: /files/content/article/2013/04/logo-color-borders@2x.jpg
[shifting-colours]: /minutae/2013/04/shifting-colors/
[site-articles]: /articles/archive/
[site-blog]: /blog/archive/
[site-minutae]: /minutae/archive/
[site-pages-about]: /about/
[site-pages-colophon]: /about/colophon/
[sitemap]: /sitemap.xml
[vscode-markdownlint]: https://marketplace.visualstudio.com/items?itemName=DavidAnson.vscode-markdownlint
[vscode]: https://code.visualstudio.com