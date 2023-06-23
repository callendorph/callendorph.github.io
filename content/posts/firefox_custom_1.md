---
title: "Firefox Customization - URL Bar"
date: 2023-06-23T14:30:47-07:00
draft: true
---

Firefox allows customization of the browser's look and feel. The [userchrome.org](https://www.userchrome.org/) has a bunch of content about how to make this change.

1.  See [this page](https://www.userchrome.org/how-create-userchrome-css.html) for creating a `userChrome.css` file.
	1.  Don't forget to enable customization by setting `toolkit.legacyUserProfileCustomizations.stylesheets` configuration to true.
2.  Add content to the `userChrome.css` file. For example, increasing the size of the URL bar's font.

```css
#urlbar {font-size: 20pt !important}
```

#  How to find more information about what can be tweaked?

You can follow the instructions in the firefox documentation for accessing the [Browser Toolbox](https://firefox-source-docs.mozilla.org/devtools-user/browser_toolbox/index.html). This gives you a debug interface similar to the standard developer tools for webpages but for the entire Firefox browser window.

<figure class="page-figure">
<img width="500rem" src="/images/BrowserToolbox.png">
<figcaption> Browser Toolbox Excerpt. </figcaption>
</figure>

You can look through the XML here to determine what elements are modifiable in the `userChrome.css` file.
