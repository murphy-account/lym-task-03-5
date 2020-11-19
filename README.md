# 3-5作业
## 1、Vue 3.0 性能提升主要是通过哪几方面体现的？
- typescript重写，可读性更强
- compositionAPI ，为复杂度高的大型项目作的优化，基于函数，让一个功能的代码放到一起。
- 响应式系统用的proxy，性能比object.defineProperty更强。
- vite,不用打包既可运行，提升开发速度。  
## 2、Vue 3.0 所采用的 Composition Api 与 Vue 2.x使用的Options Api 有什么区别？
- Options Api的同一个逻辑下的代码需要拆分到不同部分比如data,created,mounted等，而compositionAPI可以把统一逻辑下的代码放到一起，可读性复用性更强。
## 3、Proxy 相对于 Object.defineProperty 有哪些优点？
- Proxy 可以直接监听对象而非属性；
- Proxy 可以直接监听数组的变化；
## 4、Vue 3.0 在编译方面有哪些优化？
- Vue 2.x中通过标记静态根节点，优化diff 的过程，而3.0标记和提升所有的静态根节点
## 5、Vue.js 3.0 响应式系统的实现原理？
- 用Proxy取代Object.defineProperty
