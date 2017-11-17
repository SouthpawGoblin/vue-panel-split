# vue-panel-split
A split-panel component with draggable splitter for Vue.js, can be either horizontal or vertical.

## Install
```npm
npm install vue-panel-split --save
```

## Usage
```html
<template>
    <div class="app">
        <split-panel :layout="'horizontal'" :gutter="10" :init="30" :min="10" :max="90">
            <div slot="1">
                I'm panel 1
            </div>
            <div slot="2">
                I'm panel 2
            </div>
        </split-panel>
    </div>
</template>
<script>
import splitPanel from 'vue-panel-split'

export default {
  components: { splitPanel }
}
</script>
```

## Optional Attributes
name | description | values | default
---- | ----------- | ------ | -------
`layout` | layout of the panel | 'horizontal' or 'vertical' | 'horizontal'
`gutter` | gutter width in px | arbitrary | 5
`init` | initial width percentage of the first panel | 0 to 100 | 50
`min` | minimum width percentage of the first panel | 0 to 100 | 0
`miax` | maximum width percentage of the first panel | 0 to 100 | 100

## License
MIT

