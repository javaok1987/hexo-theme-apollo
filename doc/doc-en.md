## Meta Description

If you want to set meta description information, please set `desc` property and value to each post —— the better method is set default `desc` property to your scaffolds files, just like:

```md
title: Lorem ipsum dolor
date: 2015-12-31 14:49:13
desc: Lorem ipsum dolor sit amet, consectetur.
---

Lorem ipsum dolor sit amet, consectetur adipisicing elit. Totam, non numquam saepe ex ut. Deleniti culpa inventore consectetur nam saepe!
```

result:

```html
<meta name="description" content="Lorem ipsum dolor sit amet, consectetur.">
```

If there is no `desc` property or value, hexo-theme-apollo will use `page.title` and `page.author` instead of it. 

## H1~H6 Title

In fact, Hexo-theme-apollo only supoort two kinds of titles: h1~h3 belongs to what i called `big title`, and h4~h6 belongs to `small title`, this means that `#` and `###` have the same styles。

Why i do this? I support that an article should be short and clean, dont let visitors spend much time to recognise the blog post structure.

Another reason is that: i don't have met a great styles to distinguish between different kinds of headers.If you have gread idea about it, please let me know.

## Comment Plugin

Hexo-theme-apollo support two comment plugins: Disqus and Duoshuo. please set like this in your `theme/_config.yml`:

```yaml
disqus: seansun
```

## Danger Block

Use html tag with special class property to render block:

```html
<div class="tip">
    Lorem ipsum dolor sit
</div>
```

![danger](https://cloud.githubusercontent.com/assets/9530963/11359678/489a510c-92b9-11e5-9256-341cef6999b6.png)

## Legends

This may lead to disappointed: i don't have spacial tool to create diagrams，but just Microsoft Powerpoint。

## Last but not Least

Focus on blog posts, not blog's styles. Have fun :) !