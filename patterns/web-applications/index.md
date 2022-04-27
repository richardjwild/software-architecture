[Software Architecture](../..) > [Patterns](..) > Web Applications

---

These are patterns of structuring and distributing web applications. Web applications may be classified in two general types: server-side rendered and client-side rendered.
- [Server-side rendered](server-side-rendered) web applications are where the HTML is generated on the backend and transmitted directly to the browser to be displayed. This lends itself quite naturally to the whole page-at-a-time navigation style, although is frequently supplemented with AJAX calls to enrich the user experience. This style of web application has fallen rather out of favour.
- In server-side rendered web apps, a common way of structuring the code is the [model-view-controller](model-view-controller) pattern, where the HTTP requests are handled by controllers, passing model data to a view component which transforms the data into HTML.
- [Client-side rendered](client-side-rendered) web applications are where the HTML is generated on the front end and interaction with the backend is done through APIs. These invariably utilise some form of Javascript framework.
- The client-side rendered design lends itself quite naturally to the [single page app](single-page-app) architecture. The initial page request loads the whole app, and there are no more whole page roundtrips to the server. All subsequent interactions with the server are more akin to the behavious of a client-server application.
- A [micro frontend](micro-frontend) implements a web UI component that can be incorporated into a larger web application. Apart from the UI, it shares many similarities with the microservice pattern.
