# v-file

A Vue.js wrapper component for file uploading via button. (Vuetify friendly)

## Installation

```js
npm i v-file
```

### Browser

Include the script file, then install the component with `Vue.use(VFile);` e.g.:

```html
<script type="text/javascript" src="node_modules/vuejs/dist/vue.min.js"></script>
<script type="text/javascript" src="node_modules/v-file/dist/v-file.min.js"></script>
<script type="text/javascript">
  Vue.use(VFile);
</script>
```

### Module

```js
import VFile from '@outluch/v-file'

export default {
  components: {
    'v-file': VFile,
  },
}
```

## Usage

Once installed, it can be used in a template as simply as:

Simple Upload button

```html
<v-file @change="onChange">
  <v-btn>Upload</v-btn>
</v-file>
```

Button with icon

```html
<v-file>
  <v-btn icon>
    <v-icon>cloud_upload</v-icon>
  </v-btn>
</v-file>
```

## Props

You can use the following props

| Name     | Description                 |    Type | Default |
| -------- | --------------------------- | ------: | ------: |
| accept   | HTML input accept attribute |  String |      \* |
| name     | applies HTML name attribute |  String |    file |
| multiple | multiple files selection    | Boolean |   false |
