# vue-Public-methods
vue公用方法
* 全局函数
在入口文件main.js在vue的原型对象上添加函数
```javascript
Vue.prototype.areaTransfer = function(num){
    for(let x in DISTRICTS) {
        for(let y in DISTRICTS[x]) {
          if(num === y) {
            return DISTRICTS[x][y];
          }
        }
    }
}
```
在文件里调用
```javascript
this.areaTransfer('500240')

```










