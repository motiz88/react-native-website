---
id: drawerlayoutandroid
title: DrawerLayoutAndroid
---

React component that wraps the platform `DrawerLayout` (Android only). The Drawer (typically used for navigation) is rendered with `renderNavigationView` and direct children are the main view (where your content goes). The navigation view is initially not visible on the screen, but can be pulled in from the side of the window specified by the `drawerPosition` prop and its width can be set by the `drawerWidth` prop.

Example:

```
render: function() {
  var navigationView = (
    <View style={{flex: 1, backgroundColor: '#fff'}}>
      <Text style={{margin: 10, fontSize: 15, textAlign: 'left'}}>I'm in the Drawer!</Text>
    </View>
  );
  return (
    <DrawerLayoutAndroid
      drawerWidth={300}
      drawerPosition="left"
      renderNavigationView={() => navigationView}>
      <View style={{flex: 1, alignItems: 'center'}}>
        <Text style={{margin: 10, fontSize: 15, textAlign: 'right'}}>Hello</Text>
        <Text style={{margin: 10, fontSize: 15, textAlign: 'right'}}>World!</Text>
      </View>
    </DrawerLayoutAndroid>
  );
},
```

---

# Reference

## Props

### `children`

| Type         | Required |
| ------------ | -------- |
| `React.Node` | No       |

---

### `drawerBackgroundColor`

Specifies the background color of the drawer. The default value is white. If you want to set the opacity of the drawer, use rgba. Example:

```
return (
  <DrawerLayoutAndroid drawerBackgroundColor="rgba(0,0,0,0.5)">
  </DrawerLayoutAndroid>
);
```

| Type                            | Required |
| ------------------------------- | -------- |
| <code>null &#124; string</code> | No       |

---

### `drawerLockMode`

Specifies the lock mode of the drawer. The drawer can be locked in 3 states:

- unlocked (default), meaning that the drawer will respond (open/close) to touch gestures.
- locked-closed, meaning that the drawer will stay closed and not respond to gestures.
- locked-open, meaning that the drawer will stay opened and not respond to gestures. The drawer may still be opened and closed programmatically (`openDrawer`/`closeDrawer`).

| Type                                                                                              | Required |
| ------------------------------------------------------------------------------------------------- | -------- |
| <code>&#x27;unlocked&#x27; &#124; &#x27;locked-closed&#x27; &#124; &#x27;locked-open&#x27;</code> | No       |

---

### `drawerPosition`

Specifies the side of the screen from which the drawer will slide in.

| Type                                                   | Required |
| ------------------------------------------------------ | -------- |
| <code>&#x27;left&#x27; &#124; &#x27;right&#x27;</code> | Yes      |

---

### `drawerWidth`

Specifies the width of the drawer, more precisely the width of the view that be pulled in from the edge of the window.

| Type     | Required |
| -------- | -------- |
| `number` | No       |

---

### `keyboardDismissMode`

Determines whether the keyboard gets dismissed in response to a drag.

- 'none' (the default), drags do not dismiss the keyboard.
- 'on-drag', the keyboard is dismissed when a drag begins.

| Type                                                     | Required |
| -------------------------------------------------------- | -------- |
| <code>&#x27;none&#x27; &#124; &#x27;on-drag&#x27;</code> | No       |

---

### `onDrawerClose`

Function called whenever the navigation view has been closed.

| Type          | Required |
| ------------- | -------- |
| `() => mixed` | No       |

---

### `onDrawerOpen`

Function called whenever the navigation view has been opened.

| Type          | Required |
| ------------- | -------- |
| `() => mixed` | No       |

---

### `onDrawerSlide`

Function called whenever there is an interaction with the navigation view.

| Type                                                                                          | Required |
| --------------------------------------------------------------------------------------------- | -------- |
| <code>(event: SyntheticEvent&#x3C;T&#x3E;) =&#x3E; void &#124; Promise&#x3C;void&#x3E;</code> | No       |

---

### `onDrawerStateChanged`

Function called when the drawer state has changed. The drawer can be in 3 states:

- Idle, meaning there is no interaction with the navigation view happening at the time
- Dragging, meaning there is currently an interaction with the navigation view
- Settling, meaning that there was an interaction with the navigation view, and the navigation view is now finishing its closing or opening animation

| Type                             | Required |
| -------------------------------- | -------- |
| `(state: DrawerStates) => mixed` | No       |

---

### `renderNavigationView`

The navigation view that will be rendered to the side of the screen and can be pulled in.

| Type                       | Required |
| -------------------------- | -------- |
| `() => React.Element<any>` | Yes      |

---

### `statusBarBackgroundColor`

Make the drawer take the entire screen and draw the background of the status bar to allow it to open over the status bar. It will only have an effect on API 21+.

| Type                            | Required |
| ------------------------------- | -------- |
| <code>null &#124; string</code> | No       |

---

### `style`

| Type                                                                                                                                           | Required |
| ---------------------------------------------------------------------------------------------------------------------------------------------- | -------- |
| <code>&#124; null &#124; void &#124; T &#124; false &#124; &#x27;&#x27; &#124; \$ReadOnlyArray&#x3C;GenericStyleProp&#x3C;T&#x3E;&#x3E;</code> | No       |

## Methods

### `blur()`

```jsx
drawerLayoutAndroid.blur();
```

Native methods

---

### `closeDrawer()`

```jsx
drawerLayoutAndroid.closeDrawer();
```

Closes the drawer.

---

### `focus()`

```jsx
drawerLayoutAndroid.focus();
```

---

### `measure()`

```jsx
drawerLayoutAndroid.measure(callback);
```

**Parameters:**

| Name     | Type                                                                                             | Required | Description |
| -------- | ------------------------------------------------------------------------------------------------ | -------- | ----------- |
| callback | `( x: number, y: number, width: number, height: number, pageX: number, pageY: number, ) => void` | Yes      |             |

---

### `measureInWindow()`

```jsx
drawerLayoutAndroid.measureInWindow(callback);
```

**Parameters:**

| Name     | Type                                                               | Required | Description |
| -------- | ------------------------------------------------------------------ | -------- | ----------- |
| callback | `( x: number, y: number, width: number, height: number, ) => void` | Yes      |             |

---

### `measureLayout()`

```jsx
drawerLayoutAndroid.measureLayout(relativeToNativeNode, onSuccess, [onFail]);
```

**Parameters:**

| Name                 | Type                                                                    | Required | Description |
| -------------------- | ----------------------------------------------------------------------- | -------- | ----------- |
| relativeToNativeNode | `number`                                                                | Yes      |             |
| onSuccess            | `( left: number, top: number, width: number, height: number, ) => void` | Yes      |             |
| onFail               | `() => void`                                                            | No       |             |

---

### `openDrawer()`

```jsx
drawerLayoutAndroid.openDrawer();
```

Opens the drawer.

---

### `positions()`

```jsx
DrawerLayoutAndroid.positions();
```

---

### `setNativeProps()`

```jsx
drawerLayoutAndroid.setNativeProps(nativeProps);
```

**Parameters:**

| Name        | Type     | Required | Description |
| ----------- | -------- | -------- | ----------- |
| nativeProps | `Object` | Yes      |             |
