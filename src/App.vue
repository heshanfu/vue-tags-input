<template>
  <div id="app">
    <h2>Examples</h2>
    <hr>
    <input type="text" class="form-control" placeholder="Username" ref="tagsinput">
    <br>

    <tagsInput
      v-model="options"
      labelStyle="primary"></tagsInput>
  </div>
</template>

<script>
import TagsInput from "./TagsInput";

export default {
  name: 'App',
  data() {
    return {
      options: ['PHP', 'Javascript', 'Vue'],
      // options: 'PHP,JAVA,GO',
    };
  },
  methods: {
    // bt4call(tag, inx) {
    //   console.log(tag, inx);
      
    //   var _this = this;
    //   setTimeout(() => {
    //     if (tag == 1) {
    //       _this.$refs.bs4.removeTag(inx)
    //     }
    //   }, 1000);

    //   return true;
    // },
    // setTag() {
    //   var tags = ['D', 'E', 'F'];
    //   this.$refs.bs4.setTag(tags);
    // },
    // getTag() {
    //   console.log(this.$refs.bs4.getTag());
    // },
    // clearTag() {
    //   this.$refs.bs4.clearTag();
    // }
  },
  components: {
    TagsInput
  }
}
</script>

<style>
@import "https://cdn.bootcss.com/twitter-bootstrap/4.1.3/css/bootstrap.min.css";
/* @import "https://cdn.bootcss.com/twitter-bootstrap/3.3.7/css/bootstrap.min.css"; */
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  margin: 60px;
}
</style>
