# create-pixel

Helper function to reate data-uri of a one pixel image with custom color

# Credits

Copied from unkown author from this SO answer: https://stackoverflow.com/a/33919020/1644131

# Setup

With `npm`:

```
npm install create-pixel
```

With `yarn`:

```
yarn add create-pixel
```

# Usage

```js
import createPixel from 'create-pixel'

// Other option with a number: createPixel(0xff0000)
const dataUri = createPixel(`#ff0000`)

// Use in a generated image src:
const onePixelImage = new Image()
onePixelImage.src = dataUri
document.body.appendChild(onePixelImage)

// Or in a JSX component:
<img src={dataUri} />
```
