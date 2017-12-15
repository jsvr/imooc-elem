## vue-resource

### http请求动态获取数据

```javascript
// data里初始化定义把数据变量
// created钩子函数里动态请求渲染数据
data() {
      return {
        ratings: [],
        selectType: ALL,
        onlyContent: true
      };
    }
    
created() {
   this.$http.get('/api/ratings').then((response) => {
     response = response.body;
     if (response.errno === ERR_OK) {
       this.ratings = response.data;
       this.$nextTick(() => {
         this.scroll = new BScroll(this.$els.ratings, {
           click: true
         });
       });
     }
   });
 },
```