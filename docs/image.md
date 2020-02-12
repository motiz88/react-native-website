---
id: image
title: Image
---

A React component for displaying different types of images, including network images, static resources, temporary local images, and images from local disk, such as the camera roll.

See https://facebook.github.io/react-native/docs/image.html

---

# Reference

## Props

### `accessibilityLabel`

The text that's read by the screen reader when the user interacts with the image.

See https://facebook.github.io/react-native/docs/image.html#accessibilitylabel

| Type        | Required |
| ----------- | -------- |
| `Stringish` | No       |

---

### `accessible`

When true, indicates the image is an accessibility element.

See https://facebook.github.io/react-native/docs/image.html#accessible

| Type      | Required |
| --------- | -------- |
| `boolean` | No       |

---

### `blurRadius`

blurRadius: the blur radius of the blur filter added to the image

See https://facebook.github.io/react-native/docs/image.html#blurradius

| Type     | Required |
| -------- | -------- |
| `number` | No       |

---

### `capInsets`

See https://facebook.github.io/react-native/docs/image.html#capinsets

| Type                                                                                                                 | Required |
| -------------------------------------------------------------------------------------------------------------------- | -------- |
| <code>\$ReadOnly&#x3C;{&#124; bottom?: ?number, left?: ?number, right?: ?number, top?: ?number, &#124;}&#x3E;</code> | No       |

---

### `children`

| Type      | Required |
| --------- | -------- |
| `unknown` | No       |

---

### `defaultSource`

A static image to display while loading the image source.

See https://facebook.github.io/react-native/docs/image.html#defaultsource

| Type                                                                             | Required |
| -------------------------------------------------------------------------------- | -------- |
| <code>ImageURISource &#124; number &#124; Array&#x3C;ImageURISource&#x3E;</code> | No       |

---

### `fadeDuration`

| Type     | Required |
| -------- | -------- |
| `number` | No       |

---

### `height`

| Type                                                              | Required |
| ----------------------------------------------------------------- | -------- |
| <code>null &#124; number &#124; string &#124; AnimatedNode</code> | No       |

---

### `loadingIndicatorSource`

| Type                                                                       | Required |
| -------------------------------------------------------------------------- | -------- |
| <code>number &#124; \$ReadOnly&#x3C;{&#124;uri: string&#124;}&#x3E;</code> | No       |

---

### `onError`

Invoked on load error with `{nativeEvent: {error}}`.

See https://facebook.github.io/react-native/docs/image.html#onerror

| Type                                                                                                                    | Required |
| ----------------------------------------------------------------------------------------------------------------------- | -------- |
| <code>( event: SyntheticEvent&#x3C; \$ReadOnly&#x3C;{&#124; error: string, &#124;}&#x3E;, &#x3E;, ) =&#x3E; void</code> | No       |

---

### `onLayout`

Invoked on mount and layout changes with `{nativeEvent: {layout: {x, y, width, height}}}`.

See https://facebook.github.io/react-native/docs/image.html#onlayout

| Type                            | Required |
| ------------------------------- | -------- |
| `(event: LayoutEvent) => mixed` | No       |

---

### `onLoad`

Invoked when load completes successfully.

See https://facebook.github.io/react-native/docs/image.html#onload

| Type                              | Required |
| --------------------------------- | -------- |
| `(event: ImageLoadEvent) => void` | No       |

---

### `onLoadEnd`

Invoked when load either succeeds or fails.

See https://facebook.github.io/react-native/docs/image.html#onloadend

| Type         | Required |
| ------------ | -------- |
| `() => void` | No       |

---

### `onLoadStart`

Invoked on load start.

See https://facebook.github.io/react-native/docs/image.html#onloadstart

| Type         | Required |
| ------------ | -------- |
| `() => void` | No       |

---

### `onPartialLoad`

Invoked when a partial load of the image is complete.

See https://facebook.github.io/react-native/docs/image.html#onpartialload

| Type         | Required |
| ------------ | -------- |
| `() => void` | No       |

---

### `onProgress`

Invoked on download progress with `{nativeEvent: {loaded, total}}`.

See https://facebook.github.io/react-native/docs/image.html#onprogress

| Type                                                                                                                              | Required |
| --------------------------------------------------------------------------------------------------------------------------------- | -------- |
| <code>( event: SyntheticEvent&#x3C;\$ReadOnly&#x3C;{&#124;loaded: number, total: number&#124;}&#x3E;&#x3E;, ) =&#x3E; void</code> | No       |

---

### `progressiveRenderingEnabled`

| Type      | Required |
| --------- | -------- |
| `boolean` | No       |

---

### `resizeMethod`

See https://facebook.github.io/react-native/docs/image.html#resizemethod

| Type                                                                             | Required |
| -------------------------------------------------------------------------------- | -------- |
| <code>&#x27;auto&#x27; &#124; &#x27;resize&#x27; &#124; &#x27;scale&#x27;</code> | No       |

---

### `resizeMode`

Determines how to resize the image when the frame doesn't match the raw image dimensions.

See https://facebook.github.io/react-native/docs/image.html#resizemode

| Type                                                                                                                                     | Required |
| ---------------------------------------------------------------------------------------------------------------------------------------- | -------- |
| <code>&#x27;cover&#x27; &#124; &#x27;contain&#x27; &#124; &#x27;stretch&#x27; &#124; &#x27;repeat&#x27; &#124; &#x27;center&#x27;</code> | No       |

---

### `source`

The image source (either a remote URL or a local file resource).

See https://facebook.github.io/react-native/docs/image.html#source

| Type                                                                             | Required |
| -------------------------------------------------------------------------------- | -------- |
| <code>ImageURISource &#124; number &#124; Array&#x3C;ImageURISource&#x3E;</code> | No       |

---

### `src`

| Type      | Required |
| --------- | -------- |
| `unknown` | No       |

---

### `style`

See https://facebook.github.io/react-native/docs/image.html#style

| Type                                                                                                                                           | Required |
| ---------------------------------------------------------------------------------------------------------------------------------------------- | -------- |
| <code>&#124; null &#124; void &#124; T &#124; false &#124; &#x27;&#x27; &#124; \$ReadOnlyArray&#x3C;GenericStyleProp&#x3C;T&#x3E;&#x3E;</code> | No       |

---

### `testID`

A unique identifier for this element to be used in UI Automation testing scripts.

See https://facebook.github.io/react-native/docs/image.html#testid

| Type     | Required |
| -------- | -------- |
| `string` | No       |

---

### `width`

| Type                                                              | Required |
| ----------------------------------------------------------------- | -------- |
| <code>null &#124; number &#124; string &#124; AnimatedNode</code> | No       |

## Methods

### `getSize()`

```jsx
Image.getSize(uri, success, [failure]);
```

Retrieve the width and height (in pixels) of an image prior to displaying it.

See https://facebook.github.io/react-native/docs/image.html#getsize

**Parameters:**

| Name    | Type                                      | Required | Description |
| ------- | ----------------------------------------- | -------- | ----------- |
| uri     | `string`                                  | Yes      |             |
| success | `(width: number, height: number) => void` | Yes      |             |
| failure | `(error: any) => void`                    | No       |             |

---

### `getSizeWithHeaders()`

```jsx
Image.getSizeWithHeaders(uri, headers, success, [failure]);
```

Retrieve the width and height (in pixels) of an image prior to displaying it with the ability to provide the headers for the request.

See https://facebook.github.io/react-native/docs/image.html#getsizewithheaders

**Parameters:**

| Name    | Type                                      | Required | Description |
| ------- | ----------------------------------------- | -------- | ----------- |
| uri     | `string`                                  | Yes      |             |
| headers | `{[string]: string, ...}`                 | Yes      |             |
| success | `(width: number, height: number) => void` | Yes      |             |
| failure | `(error: any) => void`                    | No       |             |

---

### `prefetch()`

```jsx
Image.prefetch(url);
```

Prefetches a remote image for later use by downloading it to the disk cache.

See https://facebook.github.io/react-native/docs/image.html#prefetch

**Parameters:**

| Name | Type     | Required | Description |
| ---- | -------- | -------- | ----------- |
| url  | `string` | Yes      |             |

---

### `queryCache()`

```jsx
Image.queryCache(urls);
```

Performs cache interrogation.

See https://facebook.github.io/react-native/docs/image.html#querycache

**Parameters:**

| Name | Type            | Required | Description |
| ---- | --------------- | -------- | ----------- |
| urls | `Array<string>` | Yes      |             |
