# i386

## Requirements

* Hexo >= 3.0
* [hexo-tag-bootstrap](https://github.com/wzpan/hexo-tag-bootstrap) >= 0.0.8 (optional)

## Install

1. install theme:`git submodule add git@github.com:islongshiyu/i386.git themes/i386`
2. install [hexo-tag-bootstrap](https://github.com/wzpan/hexo-tag-bootstrap) (*optional*):`npm install hexo-tag-bootstrap --save`
3. install [hexo-generator-search](https://github.com/paichyperiondev/hexo-generator-search) (*optional*):`npm install hexo-generator-search --save`
4. create pages: i386 offers you the customized Categories, Tags and About pages. But you need to manually create these page at your 'source' folder.

For example, to create a `Categories` page, you may create a `index.html` file at `source/categories/` folder with the following contents:

```shell
---
title: Categories
layout: categories
---
```

## Enable

Modify `theme` setting in your `_config.yml` to `i386`.

## Configuration

create `_config.i386.yml` and add the follow configuration:

```shell
slogan: Yet another bootstrap theme.

menu:
  - title: Archives
    url: archives
    intro: All the articles.
    icon: fa fa-archive
  - title: Categories
    url: categories
    intro: All the categories.
    icon: fa fa-folder
  - title: Tags
    url: tags
    intro: All the tags.
    icon: fa fa-tags
  - title: About
    url: about
    intro: About me.
    icon: fa fa-user

links:
  - title: My Github
    url: http://www.github.com/blackshow
    intro: My Github account.
    icon: fa fa-github
  - title: My LinkedIn
    url: http://www.linkedin.com/in/blackshow
    intro: My Linkin account.
    icon: fa fa-linkedin

widgets:
- search
- category
- tagcloud
- recent_posts
- links

rss: atom.xml
favicon: favicon.png
fancybox: true
duoshuo_shortname:

# analytics
google_analytics:
  enable: false
  siteid:
baidu_tongji:
  enable: false
  siteid:

# Search
swiftype_key: 
```

* **slogan** - slogan display at the index page
* **menu** - Navigation menu
* **links** - reference links at the links widget
* **widgets** - Widgets displaying in sidebar
* **rss** - RSS link
* **fancybox** - Enable [Fancybox](http://fancyapps.com/fancybox/)
* **duoshuo_shortname** - DuoShuo ID, if you prefer to use duoshuo instead of Disqus
* **analytics** - Analytics ID. Supports both Google Analytics and Baidu Tongji.
* **swiftype_key** - Swifttype key to enable local searching. Leave it blank or comment this line if you want to use build-in local search engine.

If you prefer to use disqus, the setting of disqus should be placed at your **root** `_config.yml`:

## License

This theme is provided under [MIT License](http://opensource.org/licenses/MIT).
