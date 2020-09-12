# Web Scraping with Javascript and NodeJS
https://www.scrapingbee.com/blog/web-scraping-javascript/

* there are lots of different HTTP clients that you can use for querying
  * request, axios, superagent
* for web scraping without dependencies, use RegEx (uuuugggghhhh)
  * or use an HTML parser (yay)
* Cheerio is an API of JQuery on the server side
  * does not manipulate the DOM
* JSDOM is the DOM for node
  * emulates the browser
* Puppeteer allows you to manipulate the browser programmatically

# MDN document.querySelector()
https://developer.mozilla.org/en-US/docs/Web/API/Document/querySelector

* returns the first element within the document that matches the specified selector or group of selectors. If no matches are found, null is returned
* uses css selectors:
```var el = document.querySelector(".myclass");```
* can also negate selectors:
```var el = document.querySelector("div.user-panel:not(.main) input[name='login']");```

# MDN document.querySelectorAll()
https://developer.mozilla.org/en-US/docs/Web/API/Document/querySelectorAll

* example:
```var matches = document.querySelectorAll("p");```
