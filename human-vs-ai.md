# Human VS AI

Build a Mobile App with Vue.js, ML Kit, and NativeScript

Jen Looper, Progress and Founder & CEO of Vue Vixens


## WHAT is machine learning

- [Coursera course by Andrew Ng](https://www.coursera.org/learn/machine-learning?utm_source=gg&utm_medium=sem&campaignid=685340575&adgroupid=32639001341&device=c&keyword=coursera%20machine%20learning&matchtype=p&network=g&devicemodel=&adpostion=1t1&creativeid=243289762778&hide_mobile_promo&gclid=Cj0KCQjw08XeBRC0ARIsAP_gaQAjpApM-j7gdIF2ucUsLbKXEs5TvINnsE6FAcPTNab--ERLPidHIgYaArPoEALw_wcB) (what started Coursera)


### How to make a machine learn (supervised learning)

1. Gather data
    - Training set
    - Test set
1. Catagorize training set (give data labels)
    - MechanicalTurk
1. Run test

### How to make a machine learn (**un**supervised learning)

1. Gather data
    - Training set
    - Test set
1. A self-teaching pattern-recognizing algorithm
1. Run test

### How to make a machine learn (reinforcement learning)

1. Gather data
    - Training set
    - Test set
1. A curious self-taching pattern-recognizing algorithm
    - Increase difficulty
1. Run test

### Tools

- TensorFlow
    - [Intro to TF with CodeLabs](https://codelabs.developers.google.com/codelabs/tensorflow-for-poets/#0)
- [TensorFlow.js](https://js.tensorflow.org/)
    - TF for browser and Node.js

### ML in the wild

- StitchFix = ML + human curation
    - Recommendation engine
        - Location
        - Trends
        - Season
- Scary: Surveillance cameras and identification
    - Monitor group emotions
    - Track location
- Good
    - MIT kids optimize school bus routes
    - Seeing AI (read US money for blind people)
    - Facebook Marketplace: suggesting price for item
    - Spotify: daily mixes
    - Google Translate

### DIY machine learning is hard

- Tough to get good quality data
- Lots of compute
- Lots of skillz

### Make it easy

- [Clarifai](www.clarifai.com/‎) (image recognition)
- Google Cloud Platform
- On your device with a plugin...
    - Offline
    - Custom training
    - **TensorFlow!** (well, [TensorFlow Lite](https://www.tensorflow.org/lite/)) => ML Kit

### [ML Kit](https://developers.google.com/ml-kit/)

- Data through Firebase
- Google Cloud VIsion API
- Pre-trained model


## [DEMO](https://github.com/jlooper/picme) with Vue and NativeScript   

### Tools

- ML Kit
- Firebase
- Vue
- Vuex (like Redux)

### Process

1. Why Vue for NativeScript?
    - Vue 2.0 adoption of the virutal DOM enables native mobile rendering (like Angular 2+)
    - Lightweight
1. [NativeScript Vue playground](https://nativescript-vue.org/en/docs/getting-started/playground-tutorial/)
1. Image recognition: Labradoodle VS Fried Chicken
1. Scaffold Vue app with CLI
1. Vuex to keep score