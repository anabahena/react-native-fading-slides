This is a clone of @chagasaway repo
https://github.com/chagasaway/react-native-fading-slides

Solving the issue Dynamic URL passing

https://github.com/chagasaway/react-native-fading-slides/issues/3

## React Native FadingSlides Component

Simple looped fading slides carousel for React Native.

![alt tag](http://i.giphy.com/l41lR24WgEwYTaHzW.gif)

### Installation

```bash
npm install react-native-fading-slides
```

### Properties

```
fadeDuration={500} // Milliseconds for slide fade
stillDuration={1000} // Milliseconds for slide still
height={1000} // Set the slides component height
slides={slidesList} // Set the slides list
```

### Slides Properties

```
title={"Title"} // Slide's title
titleColor={"#fff"} // Slide's title color
subtitle={"Subtitle"} // Slide's subtitle
subtitleColor={"#fff"} // Slide's subtitle color
image={require('image!filename')} // Slide's image
imageWidth={1000} // Slide's image width
imageHeight={1000} // Slide's image height
```

### Usage Example

```javascript
'use strict';

var FadingSlides = require('react-native-fading-slides');

var slides = [
    {
        image: 'https://facebook.github.io/react/img/logo_og.png',
        imageWidth: 100,
        imageHeight: 100,
        title: 'Hello World',
        subtitle: 'This is a beautiful world',
        titleColor: '#fff',
        subtitleColor: '#fff'
    },
    {
        image:  'https://facebook.github.io/react/img/logo_og.png',
        imageWidth: 200,
        imageHeight: 100,
        title: 'Bye World',
        subtitle: 'This is a see you soon',
        titleColor: '#fff',
        subtitleColor: '#fff'
    }
];

//...

render: function() {
  return (
    <View>
      <FadingSlides
      slides={slides}
      fadeDuration={1200}
      stillDuration={2000}
      height={500}/>
    </View>
  );
};
```
