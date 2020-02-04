---
id: switch
title: Switch
---

Renders a boolean input.

This is a controlled component that requires an `onValueChange` callback that updates the `value` prop in order for the component to reflect user actions. If the `value` prop is not updated, the component will continue to render the supplied `value` prop instead of the expected result of any user actions.

```SnackPlayer name=switch
import React, { useState } from 'react';
import { Text, View, Switch } from 'react-native';

export default function App() {
  const [value, setValue] = useState(false);
  return (
    <View style={{ flex: 1, justifyContent: 'center', alignItems: 'center' }}>
      <Switch
        value={value}
        onValueChange={v => {
          setValue(v);
        }}
      />
    </View>
  );
}
```

---

<!--DO NOT EDIT THIS PART-->
<!--APIREF:Libraries/Components/Switch/Switch.js-->

# Reference

> **NOTE**: The API documentation for this component is generated from the React Native source code. You can edit it in [Libraries/Components/Switch/Switch.js](Libraries/Components/Switch/Switch.js).
