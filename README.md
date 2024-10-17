# hurock
A classic sidebar Hugo theme

[My personnal Hugo blog](https://titi.github.io/)

# Screenshots

Home page links:

<img src="https://raw.githubusercontent.com/titi/hurock/master/images/screenshot1.png" width="800" />

Home page posts:

<img src="https://raw.githubusercontent.com/titi/hurock/master/images/screenshot.png" width="800" />

List view:

<img src="https://raw.githubusercontent.com/titi/hurock/master/images/screenshot2.png" width="800" />

Content view:

<img src="https://raw.githubusercontent.com/titi/hurock/master/images/screenshot3.png" width="800" />

404 error page:

<img src="https://raw.githubusercontent.com/titi/hurock/master/images/screenshot4.png" width="800" />

Mobile:

<img src="https://raw.githubusercontent.com/titi/hurock/master/images/screenshot5.png" />

# Concept

* No external ressources (js/css/fonts)
* Easy to add stuff in header/footer
* Syntax highlight on client side using [highlight.js](https://highlightjs.org/)
* Responsive design
* Shortcodes for vimeo/youtube/gist
* W3C valid
 * Clean HTML
 * Sidebar after content
 * CSS in head, JS before end of body
* Fun 404 page!

Theme mostly insipred on theme `nofancy` but also: `hyde-x`, `lanyon`, `liquorice`, `purehugo`, `redlounge`.

# Config

``` toml
baseurl = "http://example.com"
title = "Your site title"

[params]
  Description = "text under logo"
  # Optional
  disqusShortname = ""
  gtagID = "Google Analytics Tracking ID"
  highlight_theme = "tomorrow-night"
  notoc = true
  [params.author]
    name = "Your Name"
    email = ""
  
    github = ""
    twitter = ""
    facebook = ""
    linkedin = ""

# Optional sections:
[permalinks]
  posts = "/:year/:month/:filename/"

[blackfriday]
  plainIdAnchors = true
```

* You can change the `highlight.js` theme, see `highlight_theme` parameter, but you'll have to add the corresponding css in your `static/highlight/` folder.
* `notoc` means no TableOfContents. It is used to hide the table of contents. Indeed, in case you're using the permalinks parameter, the table of contents links are not working with current Hugo version (0.13).
