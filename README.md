# react-image-lazy-load
React image lazy loading component inspired by [Polymer's Iron Image](https://www.webcomponents.org/element/PolymerElements/iron-image)

## How to use

1. **npm install react-image-lazy-load**
2. You will need 2 different images
    - First one will be image you want to display once it's loaded. ( Image in full HD)
    - Second is copy of the first image scaled down to **1%.** ( Image that will be displayed until the full HD image is loaded)
3. Your code should look something like  :arrow_down:

```javascript
import React from 'react'; // Import react
import IronImage from 'react-image-lazy-load'; // Install npm react lazy load package

// Images
import image from './iron-image-small.jpg'; // Low quality image ( Scaled down to 1% of it's original size )
const hdUrl = 'https://images.unsplash.com/photo-1478562853135-c3c9e3ef7905'; // Full hd image


const App = () => (
  <div>
      <IronImage alt="Enter alt text" placeholder={image} src={hdUrl} />
  </div>
);

export default App;
```
### Congrats! You made it  :tada:

![alt Lazy load image preview](https://cdn-images-1.medium.com/max/800/1*st2DLLQ2Sx1fdj1bcwuROQ.gif)

If you want to start from scratch and create your own lazy-load component check out our Medium [blog post](https://medium.com/jsguru/react-image-lazy-loading-component-246e0cdcce02)

