<template>
  <div id="app">
    <router-view></router-view>
  </div>
</template>

<script>
export default {
  name: 'app',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  }
}
</script>

<style>
  a, a:hover, a:visited, a:active {
    text-decoration: none;
  }

  body, p, ul, h1, h2, h3, h4, h5, h6 {
    margin: 0;
    padding: 0;
  }

  .clearfix:before,  .clearfix:after {
    content: " ";
    display: table;
  }
  .clearfix:after {
     clear: both;
   }

  .ico-dis {
    position: absolute;
    right: -14px;
    top: 13px;
    display: inline-block;
    width: 0;
    height: 0;
    line-height: 0;
    cursor: pointer;
    border: 5px solid;
    border-color: #999 transparent transparent transparent;
  }

  ul {
    list-style: none;
  }
</style>
