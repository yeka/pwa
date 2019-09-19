# PWA Testing Ground

This is my testing ground for learning PWA, specifically for learning the Service Worker.

Being a backend developer for years, I found it easier to develop an API service that handle a JSON request/response (or gRPC if you will). I can focus on the business logic without worrying about how the client would present it. No server side rendering.
Thus the client, be it a web browser or a mobile application (Android or IOS), can call the same API and focus on how to present it to the user.

And with my shallow knowledge on the frontend area, here I am thinking how to built a website and wondering how would it work with SEO and Tracking.
Without server side rendering, the website would be a web applications. The Javascript would do the heavy load of rendering the pages based on data it gets from API. The problem is, because the page is rendered client side, how would a search engine crawler got the SEO data?


Enter service worker.

![Service Worker][service-worker]

Service worker can work as traffic controller. It can intercept request to network and serve the page from cache instead. That way, it can also work in offline mode.

Area to explore:
1. fetch JSON from API, render it in client (using service worker) and return rendered HTML page
2. tracking user behaviour when offline


[service-worker]: ./docs/service-worker.svg