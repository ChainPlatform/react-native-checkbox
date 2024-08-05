# React Native Checkbox
@chainplatform/checkbox is a React Native library that provides a Checkbox component for react-native and react-native-web.

<a href="https://npmjs.com/package/@chainplatform/checkbox">
  <img src="https://img.shields.io/npm/v/@chainplatform/checkbox.svg"></img>
  <img src="https://img.shields.io/npm/dt/@chainplatform/checkbox.svg"></img>
</a>
<a href="https://twitter.com/intent/follow?screen_name=doansan"><img src="https://img.shields.io/twitter/follow/doansan.svg?label=Follow%20@doansan" alt="Follow @doansan"></img></a>

### Install
```
npm install @chainplatform/checkbox --save
```
or
```
yarn add @chainplatform/checkbox
```


### Usage

```js
import React from 'react';
import {StyleSheet} from 'react-native';
import CheckBox from '@chainplatform/checkbox';

class App extends React.Component {

  render() {
    return (
      <View style={{flex:1}}>
            <CheckBox
                    onClick={() => {
                        this.setState({isChecked: true});
                    }}
                    isChecked={this.state.isChecked}
                    text={"Check Box"}
                    textStyle={{
                        fontSize: 14,
                        marginLeft: 3,
                        color: "green"
                    }}
                    textAlign={'right'}
                />
      </View>
    );
  }
}
```