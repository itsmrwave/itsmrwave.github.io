---
title: "Handling MODX conditionals efficiently"
link: http://modx.com/blog/2012/09/14/tags-as-the-result-or-how-conditionals-are-like-mosquitoes/
category: minutae
layout: post
---

### Build tags as a result of a conditional, not in conditional results

An example using conditional filter expressions that have multiple conditional
paths. Here is a simple conditional that can quickly become a drain on
performance because of the order of parsing;

```
[[*field:is=`0`:then=`[[!SomeScript]]`:else=`[[$SomeChunk]]`]]
```

When MODX parses this tag, each of the tags contained in the then and the else
conditional paths are parsed, The `*field` tag itself is parsed and finally, the
conditional filter is applied. In other words, regardless of the result of your
conditional comparison, everything in both conditional paths is executed
recursively to it's logical end!

How big of an unnecessary burden this becomes depends entirely on the nature of
the tags involved. But you can see how it can quickly get out of control when
many conditionals are involved.

The brilliantly simple way to avoid this problem? Just return what's between the
MODX tags and have the result of your conditional build what is going to be
parsed next by MODX.

```
[[[[*field:is=`0`:then=`!SomeScript`:else=`$SomeChunk`]]]]
```

MODX shouldn't take your tags and run with them when embedded as results in
conditional paths. Make it wait until you've evaluated your condition to do
anything about it.

---

1. [Example of optimizing conditional filters using a Chunk wrapper][link1]
2. Check out the [comments][link2] on the original post as well

[link1]: https://gist.github.com/opengeek/3744346
[link2]: http://modx.com/blog/2012/09/14/tags-as-the-result-or-how-conditionals-are-like-mosquitoes/#comments

