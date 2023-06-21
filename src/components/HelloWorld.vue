<template>
  <div class="hello">
    <h2>东哥哥无敌666</h2>
    <magic-editor :config="config" />
  </div>
</template>

<script>
// 引入组件
import MagicEditor from "magic-editor";
// 引入样式
import "magic-editor/dist/magic-editor.css";
export default {
  name: "HelloWorld",
  components: {
    MagicEditor,
  },
  data() {
    return {
      msg: "Welcome to Your Vue.js App",
      config: {
        baseURL: "http://localhost:9999/magic/web", //配置后台服务
        serverURL: "http://localhost:9999/", //配置接口实际路径
        // 其它配置请参考文档
      },
    };
  },
};
</script>

<style scoped>
.hello {
  height: 800px;
}
</style>
