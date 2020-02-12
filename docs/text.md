---
id: text
title: Text
---

A React component for displaying text.

See https://facebook.github.io/react-native/docs/text.html

---

# Reference

## Props

### `accessibilityHint`

| Type        | Required |
| ----------- | -------- |
| `Stringish` | No       |

---

### `accessibilityLabel`

| Type        | Required |
| ----------- | -------- |
| `Stringish` | No       |

---

### `accessibilityRole`

| Type                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                | Required |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------- |
| <code>&#124; &#x27;none&#x27; &#124; &#x27;button&#x27; &#124; &#x27;link&#x27; &#124; &#x27;search&#x27; &#124; &#x27;image&#x27; &#124; &#x27;keyboardkey&#x27; &#124; &#x27;text&#x27; &#124; &#x27;adjustable&#x27; &#124; &#x27;imagebutton&#x27; &#124; &#x27;header&#x27; &#124; &#x27;summary&#x27; &#124; &#x27;alert&#x27; &#124; &#x27;checkbox&#x27; &#124; &#x27;combobox&#x27; &#124; &#x27;menu&#x27; &#124; &#x27;menubar&#x27; &#124; &#x27;menuitem&#x27; &#124; &#x27;progressbar&#x27; &#124; &#x27;radio&#x27; &#124; &#x27;radiogroup&#x27; &#124; &#x27;scrollbar&#x27; &#124; &#x27;spinbutton&#x27; &#124; &#x27;switch&#x27; &#124; &#x27;tab&#x27; &#124; &#x27;tablist&#x27; &#124; &#x27;timer&#x27; &#124; &#x27;toolbar&#x27;</code> | No       |

---

### `accessibilityState`

| Type                                                                                                                                          | Required |
| --------------------------------------------------------------------------------------------------------------------------------------------- | -------- |
| <code>{ disabled?: boolean, selected?: boolean, checked?: ?boolean &#124; &#x27;mixed&#x27;, busy?: boolean, expanded?: boolean, ... }</code> | No       |

---

### `accessible`

Indicates whether the view is an accessibility element.

See https://facebook.github.io/react-native/docs/text.html#accessible

| Type      | Required |
| --------- | -------- |
| `boolean` | No       |

---

### `adjustsFontSizeToFit`

Whether font should be scaled down automatically.

See https://facebook.github.io/react-native/docs/text.html#adjustsfontsizetofit

| Type      | Required |
| --------- | -------- |
| `boolean` | No       |

---

### `allowFontScaling`

Whether fonts should scale to respect Text Size accessibility settings.

See https://facebook.github.io/react-native/docs/text.html#allowfontscaling

| Type      | Required |
| --------- | -------- |
| `boolean` | No       |

---

### `children`

| Type   | Required |
| ------ | -------- |
| `Node` | No       |

---

### `dataDetectorType`

| Type                                                                                                                                 | Required |
| ------------------------------------------------------------------------------------------------------------------------------------ | -------- |
| <code>&#x27;phoneNumber&#x27; &#124; &#x27;link&#x27; &#124; &#x27;email&#x27; &#124; &#x27;none&#x27; &#124; &#x27;all&#x27;</code> | No       |

---

### `disabled`

Specifies the disabled state of the text view for testing purposes.

See https://facebook.github.io/react-native/docs/text.html#disabled

| Type      | Required |
| --------- | -------- |
| `boolean` | No       |

---

### `ellipsizeMode`

When `numberOfLines` is set, this prop defines how text will be truncated.

See https://facebook.github.io/react-native/docs/text.html#ellipsizemode

| Type                                                                                                    | Required |
| ------------------------------------------------------------------------------------------------------- | -------- |
| <code>&#x27;clip&#x27; &#124; &#x27;head&#x27; &#124; &#x27;middle&#x27; &#124; &#x27;tail&#x27;</code> | No       |

---

### `maxFontSizeMultiplier`

Specifies largest possible scale a font can reach when `allowFontScaling` is enabled. Possible values: `null/undefined` (default): inherit from the parent node or the global default (0) `0`: no max, ignore parent/global default `>= 1`: sets the maxFontSizeMultiplier of this node to this value

| Type     | Required |
| -------- | -------- |
| `number` | No       |

---

### `minimumFontScale`

Smallest possible scale a font can reach.

See https://facebook.github.io/react-native/docs/text.html#minimumfontscale

| Type     | Required |
| -------- | -------- |
| `number` | No       |

---

### `nativeID`

Used to locate this view from native code.

See https://facebook.github.io/react-native/docs/text.html#nativeid

| Type     | Required |
| -------- | -------- |
| `string` | No       |

---

### `numberOfLines`

Used to truncate the text with an ellipsis.

See https://facebook.github.io/react-native/docs/text.html#numberoflines

| Type     | Required |
| -------- | -------- |
| `number` | No       |

---

### `onLayout`

Invoked on mount and layout changes.

See https://facebook.github.io/react-native/docs/text.html#onlayout

| Type                            | Required |
| ------------------------------- | -------- |
| `(event: LayoutEvent) => mixed` | No       |

---

### `onLongPress`

This function is called on long press.

See https://facebook.github.io/react-native/docs/text.html#onlongpress

| Type                           | Required |
| ------------------------------ | -------- |
| `(event: PressEvent) => mixed` | No       |

---

### `onMoveShouldSetResponder`

| Type            | Required |
| --------------- | -------- |
| `() => boolean` | No       |

---

### `onPress`

This function is called on press.

See https://facebook.github.io/react-native/docs/text.html#onpress

| Type                           | Required |
| ------------------------------ | -------- |
| `(event: PressEvent) => mixed` | No       |

---

### `onResponderGrant`

| Type                                              | Required |
| ------------------------------------------------- | -------- |
| `(event: PressEvent, dispatchID: string) => void` | No       |

---

### `onResponderMove`

| Type                          | Required |
| ----------------------------- | -------- |
| `(event: PressEvent) => void` | No       |

---

### `onResponderRelease`

| Type                          | Required |
| ----------------------------- | -------- |
| `(event: PressEvent) => void` | No       |

---

### `onResponderTerminate`

| Type                          | Required |
| ----------------------------- | -------- |
| `(event: PressEvent) => void` | No       |

---

### `onResponderTerminationRequest`

| Type            | Required |
| --------------- | -------- |
| `() => boolean` | No       |

---

### `onStartShouldSetResponder`

| Type            | Required |
| --------------- | -------- |
| `() => boolean` | No       |

---

### `onTextLayout`

| Type                                | Required |
| ----------------------------------- | -------- |
| `(event: TextLayoutEvent) => mixed` | No       |

---

### `pressRetentionOffset`

Defines how far your touch may move off of the button, before deactivating the button.

See https://facebook.github.io/react-native/docs/text.html#pressretentionoffset

| Type                                                                                                         | Required |
| ------------------------------------------------------------------------------------------------------------ | -------- |
| <code>\$ReadOnly&#x3C;{&#124; top: number, left: number, bottom: number, right: number, &#124;}&#x3E;</code> | No       |

---

### `selectable`

Lets the user select text.

See https://facebook.github.io/react-native/docs/text.html#selectable

| Type      | Required |
| --------- | -------- |
| `boolean` | No       |

---

### `selectionColor`

The highlight color of the text.

See https://facebook.github.io/react-native/docs/text.html#selectioncolor

| Type     | Required |
| -------- | -------- |
| `string` | No       |

---

### `style`

| Type                                                                                                                                           | Required |
| ---------------------------------------------------------------------------------------------------------------------------------------------- | -------- |
| <code>&#124; null &#124; void &#124; T &#124; false &#124; &#x27;&#x27; &#124; \$ReadOnlyArray&#x3C;GenericStyleProp&#x3C;T&#x3E;&#x3E;</code> | No       |

---

### `suppressHighlighting`

When `true`, no visual change is made when text is pressed down.

See https://facebook.github.io/react-native/docs/text.html#supperhighlighting

| Type      | Required |
| --------- | -------- |
| `boolean` | No       |

---

### `testID`

Used to locate this view in end-to-end tests.

See https://facebook.github.io/react-native/docs/text.html#testid

| Type     | Required |
| -------- | -------- |
| `string` | No       |

---

### `textBreakStrategy`

Set text break strategy on Android.

See https://facebook.github.io/react-native/docs/text.html#textbreakstrategy

| Type                                                                                       | Required |
| ------------------------------------------------------------------------------------------ | -------- |
| <code>&#x27;balanced&#x27; &#124; &#x27;highQuality&#x27; &#124; &#x27;simple&#x27;</code> | No       |
