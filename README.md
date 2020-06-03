## vue-pinch
Vue 轻量级捏合、扩大手势指令。

### 安装
使用 [npm](https://www.npmjs.com/package/vue-pinch) 安装：
```git
npm i vue-pinch --save
```

```javascript
import Vue from 'vue'
import VuePinch from 'vue-pinch'

Vue.use(VuePinch)
```

### 使用

```html
<template>
    <div class="pinch" v-pinch="pinchCtrl"></div>
</template>
```

```javascript
new Vue({
  methods: {
      pinchCtrl: function (e) {        
          if(e==='pinchin'){
              console.log('捏合')
          }
          if(e==='pinchout'){
              console.log('扩大');
          }
      }
  }
})
```

#### 回调参数
- `pinchin` ：操作为捏合手势；
- `pinchout` ：操作为扩大手势；