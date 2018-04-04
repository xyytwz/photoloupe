<template>
  <div id="app">
      <div class="goodPic">
          <photoloupe class :src="goodPic" :magnification="3"></photoloupe>
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
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top:30px;
}

h1, h2 {
  font-weight: normal;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  display: inline-block;
  margin: 0 10px;
}

a {
  color: #42b983;
}
.goodPic{
    width:400px;
    height:400px;
    border:1px solid #ddd;
}
</style>
