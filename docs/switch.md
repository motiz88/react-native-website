---
id: switch
title: Switch
---

A visual toggle between two mutually exclusive states.

This is a controlled component that requires an `onValueChange` callback that updates the `value` prop in order for the component to reflect user actions. If the `value` prop is not updated, the component will continue to render the supplied `value` prop instead of the expected result of any user actions.

---

# Reference

## Props

Inherits [View Props](view.md#props).

### `disabled`

Whether the switch is disabled. Defaults to false.

| Type      | Required |
| --------- | -------- |
| `boolean` | No       |

---

### `ios_backgroundColor`

On iOS, custom color for the background. This background color can be seen either when the switch value is false or when the switch is disabled (and the switch is translucent).

| Type               | Required |
| ------------------ | -------- |
| [color](colors.md) | No       |

---

### `onChange`

Called when the user tries to change the value of the switch.

Receives the change event as an argument. If you want to only receive the new value, use `onValueChange` instead.

| Type                                                                                | Required |
| ----------------------------------------------------------------------------------- | -------- |
| <code>(event: SwitchChangeEvent) =&#x3E; Promise&#x3C;void&#x3E; &#124; void</code> | No       |

---

### `onValueChange`

Called when the user tries to change the value of the switch.

Receives the new value as an argument. If you want to instead receive an event, use `onChange`.

| Type                                                                      | Required |
| ------------------------------------------------------------------------- | -------- |
| <code>(value: boolean) =&#x3E; Promise&#x3C;void&#x3E; &#124; void</code> | No       |

---

### `thumbColor`

Custom color for the switch thumb.

| Type               | Required |
| ------------------ | -------- |
| [color](colors.md) | No       |

---

### `trackColor`

Custom colors for the switch track.

NOTE: On iOS when the switch value is false, the track shrinks into the border. If you want to change the color of the background exposed by the shrunken track, use `ios_backgroundColor`.

| Type                                                                                        | Required |
| ------------------------------------------------------------------------------------------- | -------- |
| <code>\$ReadOnly&#x3C;{&#124; false?: ?ColorValue, true?: ?ColorValue, &#124;}&#x3E;</code> | No       |

---

### `value`

Boolean value of the switch. Defaults to false.

| Type      | Required |
| --------- | -------- |
| `boolean` | No       |
