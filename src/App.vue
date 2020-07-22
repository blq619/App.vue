<template>
  <div id="app"> 
    <Topbar v-bind:msg="msg" />
    {{msg}} <br> My name is {{name}}
    <br />
    <br />
    <input type="text" v-model="name" />
    <label>제목</label>
    <input type="text" v-model="msg" />
    <Bottom />
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
import Topbar from './components/Topbar';
import Bottom from './components/Bottom';


export default {
  name: 'App',
  components: {
    Topbar,
    Bottom
    // HelloWorld
  },
  data(){
    return {
      msg: "Hello Vue JS",
      name: "KukNam"
    };
  }
};
</script>

<style>
*{
 margin:0;
 padding:0;
}
.header {
  padding: 1rem 0;
  background: salmon;
  color: #fff;
  text-align: center;
}
.footer {
  width: 100%;
  padding: 1rem 0;
  position: fixed;
  text-align: center;
  bottom: 0;
  background: #333;
  color: #fff;
}

</style>
