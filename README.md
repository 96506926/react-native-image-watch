# react-native-image-fit
ImageWatch component for RN

### Installation

```sh
$ npm install --save react-native-image-watch
```
or

```sh
$ yarn add react-native-image-watch
```

### Usage

```javascript
import { ImageViewer } from 'react-native-image-watch';

export const App = () => (
  <ImageViewer
    disabled={false} // by default
    source={require('./photo.png')} // or { url: 'https://...' }
    doubleTapEnabled={true} // by default double tap will zoom image
    onMove={(e, gestureState) => null}
    onPress={(opening) => console.log(opening)}
    mainImageStyle={styles.someStyle}
    zoomedImageStyle={styles.zoomedImageStyle}
    mainImageProps={{
        resizeMode: 'contain'
    }}
    zoomedImageProps={{
        resizeMode: 'contain'
    }}
  />
)
```

