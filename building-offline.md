# Building Rich Offline Apps

Tejas Ranade (Director of Product, Kinvey)

Kinvey ~= Firebase / Parse

- Look at app storage on your mobile, many major apps store lots of data to enable offline


## Take Aways

- Abstract service adapter layer to determine if saving locally or remotely?
- Conflict resolution is hard
- Not one-size-fits-all. Implement policies and abstraction as appropriate for data use


## Use Cases

- Short period of intermittent data – MBTA Redline
- Long periods of data disconnect – Construction management or Traveling abroad


## Landscape

- Data persistence
    - Simple/small data
    - Complex/large data
- Data synchronization

Not covered in presentation

- Asset Caching / Caching API
- Service Workers


## Offline Storage Options

- iOS & Android
    - File storage
    - SQLite
        - Self contained
        - Reliable
        - Familiar syntax
        - Adapters
            - Swift wrappers (iOS)
            - Room Persistence Library (Android)
            - Plugins for JS platforms
    - Realm
        - Open source cross-platform database across iOS, Android, Xamarin, and Node
        - Encryption
- Web
    - Local Storage
        - 5mb max
        - Key/val store
        - Strings only
        - Synchronous
    - Cookies
    - IndexedDB
        - Summary
            - Optimized for large data
            - Complex data
            - Async
            - Transactional
        - Feaure: Cursors (iterator)
    - Alternatives
        - Dexie.js - IndexedDB wrapper
        - localForage
        - JsStore
        - PouchDB
        - LokiJS
            - Fast in-memory DB
            - Run in Node, NativeScript, Cordova, browser
            - Open source document-oriented db written in JS


## Data Synchronization

- Policy
    - Offline first?
    - Online attempt first?
    - Offline followed by online?
- Sync Problems
    - Only retrieve **changes**
    - Performance **and** scale (sync, batching, etc)
    - Conflict resolution
        - Nuanced - use case dictates the solution
        - Usually the backend systems (data stores) have conflict resolution policies
        - Write the conflict resolution on the data stores
        - Give user meaningful response
- Network APIs
    - `navigator.onLine`
    - Network Information API: `(navigator.connection || navigator.mozConnection || navigator.webkitConnection).addEventListener("change", () => { ... })`
    - These APIs are flakey. False negatives are likely.


## Considerations when Implementing Offline

- Level of abstraction necessary
- Amount of data being consumed
- Data sync policies
- Platform support