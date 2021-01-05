# VS Code ES7 React-Native/Reanimated2/TS snippets

This extension provides you JavaScript, TypeScript, React Native and Reanimated 2 snippets in ES7 with Babel plugin features for [VS Code](https://code.visualstudio.com/)

## Installation

### GitHub Repository Clone

Change to your `.vscode/extensions` [VS Code extensions directory](https://code.visualstudio.com/docs/extensions/install-extension#_side-loading).
Depending on your platform it is located in the following folders:

- _Linux_: `~/.vscode/extensions`
- _macOS_: `~/.vscode/extensions`
- _Windows_: `%USERPROFILE%\.vscode\extensions`

Clone the Material Theme repository as `dsznajder.es7-react-js-snippets`:

```shell
git clone https://github.com/nicoache1/vscode-es7-javascript-react-snippets nicoache1.es7-rn-reanimated2-ts-snippets
```

## Search command

You can search through snippets with `ES7 snippet search` command which can be run with `CMD + Shift + P` or just use `CMD + Shift + R` (`CTRL + ALT + R` for Windows & Linux) keybinding.

## Supported languages (file extensions)

- JavaScript (.js)
- JavaScript React (.jsx)
- TypeScript (.ts)
- TypeScript React (.tsx)

## Snippets info

Every space inside `{ }` and `( )` means that this is pushed into next line :)
`$` represent each step after `tab`.

_TypeScript_ has own components and own snippets. Use search or just type `ts` before every component snippet.

I.E. `tsrcc`

## Basic Methods

|  Prefix | Method                                              |
| ------: | --------------------------------------------------- |
|  `imp→` | `import moduleName from 'module'`                   |
|  `imn→` | `import 'module'`                                   |
|  `imd→` | `import { destructuredModule } from 'module'`       |
|  `ime→` | `import * as alias from 'module'`                   |
|  `ima→` | `import { originalName as aliasName} from 'module'` |
|  `exp→` | `export default moduleName`                         |
|  `exd→` | `export { destructuredModule } from 'module'`       |
|  `exa→` | `export { originalName as aliasName} from 'module'` |
|  `enf→` | `export const functionName = (params) => { }`       |
|  `edf→` | `export default (params) => { }`                    |
|  `met→` | `methodName = (params) => { }`                      |
|  `fre→` | `arrayName.forEach(element => { }`                  |
|  `fof→` | `for(let itemName of objectName { }`                |
|  `fin→` | `for(let itemName in objectName { }`                |
| `anfn→` | `(params) => { }`                                   |
|  `nfn→` | `const functionName = (params) => { }`              |
|  `dob→` | `const {propName} = objectToDescruct`               |
|  `dar→` | `const [propName] = arrayToDescruct`                |
|  `sti→` | `setInterval(() => { }, intervalTime`               |
|  `sto→` | `setTimeout(() => { }, delayTime`                   |
| `prom→` | `return new Promise((resolve, reject) => { }`       |
| `cmmb→` | `comment block`                                     |
|   `cp→` | `const { } = this.props`                            |
|   `cs→` | `const { } = this.state`                            |

## React

|    Prefix | Method                                                      |
| --------: | ----------------------------------------------------------- |
|    `imr→` | `import React from 'react'`                                 |
|   `imrs→` | `import React, { useState } from 'react'`                   |
|  `imrse→` | `import React, { useState, useEffect } from 'react'`        |
|  `redux→` | `import { connect } from 'react-redux'`                     |
| `rconst→` | `constructor(props) with this.state`                        |
|  `rconc→` | `constructor(props, context) with this.state`               |
|    `cdm→` | `componentDidMount = () => { }`                             |
|    `scu→` | `shouldComponentUpdate = (nextProps, nextState) => { }`     |
|   `cdup→` | `componentDidUpdate = (prevProps, prevState) => { }`        |
|   `cwun→` | `componentWillUnmount = () => { }`                          |
|  `gdsfp→` | `static getDerivedStateFromProps(nextProps, prevState) { }` |
|   `gsbu→` | `getSnapshotBeforeUpdate = (prevProps, prevState) => { }`   |

## React Hooks

- All hooks from [official docs](https://reactjs.org/docs/hooks-reference.html) are added with hook name prefix.

## React Native

|     Prefix | Method                                 |
| ---------: | -------------------------------------- |
|    `imrn→` | `import { $1 } from 'react-native'`    |
| `rnstyle→` | `const styles = StyleSheet.create({})` |

## Redux

|       Prefix | Method                    |
| -----------: | ------------------------- |
|  `rxaction→` | `redux action template`   |
|   `rxconst→` | `export const $1 = '$1'`  |
| `rxreducer→` | `redux reducer template`  |
|  `rxselect→` | `redux selector template` |
|   `rxslice→` | `redux slice template`    |

## GraphQL

|     Prefix | Method                                                  |
| ---------: | ------------------------------------------------------- |
| `graphql→` | `import { compose, graphql } from react-apollo'`        |
| `expgql->` | `export default compose(graphql($1, { name: $2 }))($3)` |

## Console

| Prefix | Method                              |
| -----: | ----------------------------------- |
| `clg→` | `console.log(object)`               |
| `clo→` | `console.log("object", object)`     |
| `ctm→` | `console.time("timeId")`            |
| `cte→` | `console.timeEnd("timeId")`         |
| `cas→` | `console.assert(expression,object)` |
| `ccl→` | `console.clear()`                   |
| `cco→` | `console.count(label)`              |
| `cdi→` | `console.dir`                       |
| `cer→` | `console.error(object)`             |
| `cgr→` | `console.group(label)`              |
| `cge→` | `console.groupEnd()`                |
| `ctr→` | `console.trace(object)`             |
| `cwa→` | `console.warn`                      |
| `cin→` | `console.info`                      |

## React Native Components

### `rnc`

```javascript
import React, { Component } from 'react'
import { Text, View } from 'react-native'

export default class FileName extends Component {
  render() {
    return (
      <View>
        <Text> $2 </Text>
      </View>
    )
  }
}
```

### `rnf`

```javascript
import React from 'react'
import { View, Text } from 'react-native'

export default function $1() {
  return (
    <View>
      <Text> $2 </Text>
    </View>
  )
}
```

### `rnfs`

```javascript
import React from 'react'
import { StyleSheet, View, Text } from 'react-native'

export default function $1() {
  return (
    <View>
      <Text> $2 </Text>
    </View>
  )
}

const styles = StyleSheet.create({})
```

### `rnfe`

```javascript
import React from 'react'
import { View, Text } from 'react-native'

const $1 = () => {
  return (
    <View>
      <Text> $2 </Text>
    </View>
  )
}

export default $1
```

### `rnfes`

```javascript
import React from 'react'
import { StyleSheet, View, Text } from 'react-native'

const $1 = () => {
  return (
    <View>
      <Text> $2 </Text>
    </View>
  )
}

export default $1

const styles = StyleSheet.create({})
```

### `rncs`

```javascript
import React, { Component } from 'react'
import { Text, StyleSheet, View } from 'react-native'

export default class FileName extends Component {
  render() {
    return (
      <View>
        <Text> $2 </Text>
      </View>
    )
  }
}

const styles = StyleSheet.create({})
```

### `rnce`

```javascript
import React, { Component } from 'react'
import { Text, View } from 'react-native'

export class FileName extends Component {
  render() {
    return (
      <View>
        <Text> $2 </Text>
      </View>
    )
  }
}

export default $1
```

### `tsrnfis`

```javascript
import React from 'react'
import { View, Text, StyleSheet } from 'react-native'

interface testProps {}

const styles = StyleSheet.create({
  container: {
    alignItems: 'center',
    flex: 1,
    justifyContent: 'center',
  },
})

export const test: React.FC<testProps> = ({}) => {
  return (
    <View style={styles.container}>
      <Text>Hi</Text>
    </View>
  )
}
```

## Reanimated

|            Prefix | Method                                           |
| ----------------: | ------------------------------------------------ |
|          `ianim→` | `import Animated from 'react-native-reanimated'` |
| `useSharedValue→` | `const value = useSharedValue<number>(0)`        |

### `useDerivedValue`

```javascript
const derivedValue = useDerivedValue(() => {
  return {}
}, [])
```

### `useAnimatedStyle`

```javascript
const animatedStyle = useAnimatedStyle(() => ({
  transform: [{ translateY: sharedValue.value }],
}))
```

### `useAnimatedProps`

```javascript
const animatedProps = useAnimatedProps(() => {
  return {}
})
```

### `animatedPanGesture`

```javascript
const gestureHandler = useAnimatedGestureHandler<
  PanGestureHandlerGestureEvent,
   { offsetY: number, offsetX: number }
>({
     onActive: ({ translationY }, context) => {
       translateY.value = translationY
     },
    onStart: (_event, context) => {
       context.offsetY = translateY.value
     },
})
```

### `animatedTapGesture`

```javascript
const tapGestureEvent = useAnimatedGestureHandler<
  TapGestureHandlerGestureEvent,
   any
>({
     onActive: () => {
       runOnJS(onPress)()
     },
})
```
