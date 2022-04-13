---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

title: Tip: Chrome Search Engine Shortcut
layout: page
---

To make it easier to lookup an HTTP status code in Google Chrome,
simply open your [Chrome search engine settings](chrome://settings/searchEngines) and define a new search engine:

* Search Engine: HTTP Status Codes
* Shortcut: `status` (or whatever you choose)
* URL with %s in place of query: `https://davidbiesack.github.io/http-status-codes/%s`

![Chrome Search Engine Settings]({{site.baseurl}}/assets/img/Google-search-shortcut.png "Chrome Search Engine Settings")

Then simply use the shortcut in the browser address bar

> status \<space\> 418

![Search with the shortcut]({{site.baseurl}}/assets/img/searching.png "Search with the shortcut")

... and Voila:

![Search Results]({{site.baseurl}}/assets/img/search-result.png "Search Results")
