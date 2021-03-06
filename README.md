# z_act
A React-like JavaScript library.

# Differences from React
- z_act is faster than React in what it does
- z_act diffs the new virtual-dom-tree with the real-dom-tree **almost like preact**.
- z_act only diffs the sub-tree which the setState event occurred in.
- z_act supports only 2 lifecycle events **componentDidMount** and **componentWillUnmount**.
- children of jsx elements must be declared in the normal html-like way and not in the props for example :
```jsx
    <parent> <child></child> </parent>
```
- z_act doesn't support refs because every statful component has a **dom** property references the dom element that represents the component.
- z_act setState method is sync

# Use z_act in the browser
```html
<script src="https://cdn.rawgit.com/ahmedyoussef70/c7cd2b220dec0230bf2bfc094d2a9e8d/raw/24c6910af50abf2a4324feed4fcb58e3a0608d86/z_act.min.js"></script>
<script src="https://unpkg.com/babel-standalone@6/babel.min.js"></script>
<script type="text/babel">
/* @jsx h */
const { h, Component, render } = z_act
    // your code ...
</script>
```

# Demos
- basic react examples re-created with z_act.js https://codepen.io/ahmedyoussef70/pen/zLPdJw
- shuffling a list of inputs with unique keys every second https://codepen.io/ahmedyoussef70/pen/zLLVVz
