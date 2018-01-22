## Components-use

### 普通引用
  - 配置代码(组件不注册没法师用)
  ```jacascript
  <!-- html -->
  <hello><hello>

  <script>
    import Hello from './components/Hello' //引入组件

    //注册组件,标签名和变量名一样时刻简写成一个名字
    export default{
        components: {
            Hello // 简写
            hello: Hello // 键:标签名; 值:变量名.
        }
    }

  </script>
  ```