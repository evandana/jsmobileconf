# Building Progressive (web) Apps

Michael Solati


## Summary

- Service Workers
    - [Browser support](https://caniuse.com/#search=service%20workers)
- Server Side Rendering
- Web App Manifest
- Set up prefetching

### Questions

- Can you do a deep link into a PWA (like a native app)?


## Should Be

- Reliable
- Fast
- Engaging


## Is it a PWA

- [Lighthouse](https://developers.google.com/web/ilt/pwa/lighthouse-pwa-analysis-tool)!
    - Node module
    - Chrome DevTools


## PWA Requisites

- Register Service Workers
- Respond with 200 even when offline
- Fallback when JS is not available
- Prompt to install
- Custom splash screen
- Finish rendering within 5s (for SEO crawling)
- Address bar color matches brand colors
- Caching
- Push notifications


## Make it Reliable: **Service Workers**

- Caches data for offline use
- [Google Service Workers](https://developers.google.com/web/fundamentals/primers/service-workers/)
- [MDN Service Worker API](https://developer.mozilla.org/en-US/docs/Web/API/Service_Worker_API)
- Packages available for JS frameworks
    - [Polymer](https://www.polymer-project.org/1.0/toolbox/service-worker)


## Make it Fast: **Server Side Rendering**

- [react](http://reactjs.org/docs/react-dom-server.html)
- Cloud Functions for Firebase
    - Cache with CDN
- Check your site with JS disabled
    - Simulates SEO viewing


## Make it Engaging: **Web App Manifest**

### Implement in HTML Header

- `<link rel="manifest" href="FILE.json">`


### Features

- Installable
- Web push notification
- Icon

### References

- [MDN Manifest API](https://developer.mozilla.org/en-US/docs/Web/Manifest)
- [Web App Manifest Generator](https://app-manifest.firebaseapp.com/)