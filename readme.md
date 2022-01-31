# Base HTML


## Install DS
```bash
npm i storybook-html-demo -D
```

```bash
cd node_modules/storybook-html-demo && npm i
```

run this command to run storybook `npm explore storybook-html-demo -- npm run storybook`

## Add a Storybook Design System
To add a Design System made with storyboook you can do it by updating the `./storybook/main.js`

```javascript
  "refs": {
    "design-system": {
      "title": "iLab Design System",
      "url": "https://main--61d37f5ad4221d003aab534d.chromatic.com/",
      "expanded": false, // optional, true by default
    }
  }
```



# Link the css
```HTML
<link rel="stylesheet" href="index.css">
```

# In the scss file import the DS css file
```css
@import "../node_modules/storybook-html-demo/src/stories/atoms/Button.css";
@import "../node_modules/storybook-html-demo/src/stories/molecules/ButtonGroup.css";
```
# Run CSS
```bash
sass --style=compressed ./src/index.scss ./src/index.css
```
