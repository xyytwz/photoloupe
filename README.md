# photoloupe

> 图片放大器

## Build Setup

``` bash
# install dependencies
npm install

# serve with hot reload at localhost:8080
npm run dev

# build for production with minification
npm run build
```


For detailed explanation on how things work, consult the [docs for vue-loader](http://vuejs.github.io/vue-loader).

## 引用示例：
``` bash
<template>
  <div id="app">
      <div class="goodPic">
          <photoloupe class :src="goodPic" :magnification="1.5"></photoloupe>
      </div>
  </div>
</template>

<script>
import goodPic from "./assets/godPic1.jpg";
import photoloupe from './components/photoloupe'
export default {
  name: 'app',
  components:{
      photoloupe
  },
  data () {
    return {
      goodPic:goodPic
    }
  }
}
</script>

<style>
.goodPic{
    width:400px;
    height:400px;
    border:1px solid #ddd;
}
</style>
``` 

## 参数说明：

参数 | 说明 | 默认值|备注
---|---|---|---
src | 图片路径|defaultImg.png|
width | 图片宽度|400|宽高比例可以调整
height | 图片高度|400|宽高比例可以调整
magnification|放大倍数|2|最小为1，支持小数
