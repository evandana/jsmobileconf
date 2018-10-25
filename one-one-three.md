# One Project. One Language. Three Apps.

TJ VanToll (@tjvantoll), Progress

- iOS
- Web
- Android

**Solutions**

- [React Native](http://www.reactnative.com/)
- [NativeScript](https://www.nativescript.org/)


## Background

[Web VS Native](https://www.progress.com/blogs/choose-between-progressive-web-apps-react-native-nativescript-2018)

- Native Apps: 90% of **time** on phones, 77% of **time** on tablets
- Web: 2.2x more monthly **unique** visitors than average mobile app


## TakeAway

- NativeScript
    - Bifurcated code
    - Angular
- React Native
    - React
    - Simpler


## Approaches

- Both
    - Markup is **not** HTML
    - Support Flexbox
    - CSS irregularities: `float` and `display` are tough to work into Native
- React Native Web
    - Getting started: use the [Code Sandbox](https://codesandbox.io/s/q4qymyp2l6)
    - Use API from "react-native" library (e.g. `<SafeAreaView>` instead of `<div>`)
    - `fetch` method done with **Native** API (web, iOS, Android)
    - Example of bifurcation of features: Offline
        - Web: `localstorage`
        - Mobile: files
        - Solutions:
            1. Conditional logic (different code block or file)
            1. `AsyncStorage` from "react-native"
    - Generated code is UGLY (massive nesting and class lists)
    - [Compatibility from Native to Web](https://github.com/necolas/react-native-web#user-content-components)
    - Same components rendering to all three
- NativeScript Schematics
    - "schematics" means extension API for building for all three platforms
    - Use Angular CLI
        - Preview Web: `ng serve`
        - Android: `tns run android --hmr`
        - iOS: `tns run ios --hmr`
    - Fork markup and styles for each platform (web and mobile)
    - Supports SASS
    - Platform feature bifurcation
        1. Define a common component name (e.g. 'bifurcHelper')
        1. Platform-specific files get unique implementation details for this
    - [Marketplace](https://market.nativescript.org/)