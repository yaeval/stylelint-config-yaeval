# stylelint-config-yaeval

This stylelint configuration covers many commonly used CSS properties and sorts them.

Sort order:

- `position`
- `display`
- `flex & grid`
- `box model`
- `background`
- `foreground`
- `list & table`
- `transform & animation`
- `other`

If you have any suggestions, create an issue.

## Installation & Usage

First install the package:

```sh
npm install stylelint-config-yaeval
```

Then in your stylelint config file (javascript config example):

```javascript
module.exports = {
  extends: ['stylelint-config-standard'],
  // ...
}
```

## Before

```css
.element {
  bottom: 0;
  margin: 0;
  visibility: visible;
  display: flex;
  left: 0;
  outline: none;
  z-index: 1;
  position: static;
  flex: 1;
  padding: 0;
  opacity: 1;
  content: '';
  right: 0;
  top: 0;
  border: none;
}
```

## After

```css
.element {
  position: static;
  top: 0;
  right: 0;
  bottom: 0;
  left: 0;
  z-index: 1;
  display: flex;
  visibility: visible;
  flex: 1;
  margin: 0;
  outline: none;
  border: none;
  padding: 0;
  opacity: 1;
  content: '';
}
```
