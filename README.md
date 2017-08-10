# react-native-wayne-checkboxlist
React-native版单多选的listview，适配IOS和Android
这是采用的ES6新语法写的,此组件基于react-native-checkoutbox

##安装
```sh
npm install react-native-wayne-checkboxlist --save
```
##使用

这里是组件使用的概述。

```jsx
import CheckboxList from 'react-native-wayne-checkboxlist'
```

##使用示例1

```jsx
<CheckboxList
    options={[
    'Lorem ipsum dolor sit',
    'Lorem ipsum',
    'Lorem ipsum dolor sit amet, consetetur sadipscing elitr',
    'Lorem ipsum dolor sit amet, consetetur'
    ]}
    selectedOptions={['Lorem ipsum']}
    maxSelectedOptions={2}
    onSelection={(option)=>alert(option + ' was selected!')}
/>
```

##属性

* `style - {}` custom style of the list
* `optionStyle - {}` custom style of the option element
* `options - []` required array of options
* `selectedOptions - []` optional array of initially selected options
* `maxSelectedOptions - int` optional maximum number of selectable options
* `onSelection - function(option){}` option selection callback
* `renderIndicator - function(option)` should return a selected/deselected indicator node, default: check mark image
* `renderSeparator - function(option)` should return a separator node that is displayed between the options, default: gray line
* `renderText - function(option)` should return a text node, default: text node
* `renderRow - function(option)` should return a option view
* `disabled - bool` if set to true component is disabled and can't be interacted with

##截图

![example](https://github.com/wayne214/react-native-wayne-checkboxlist/blob/master/checkboxlist.png)
