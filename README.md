# vue-scroll
scroll directive for [vuejs 2.0](https://vuejs.org/v2/guide/)

For vue 1.x, please use vue-scroll@1.0.4. Currently its code is in master branch.

[![NPM](https://nodei.co/npm/vue-scroll.png?stars&downloads)](https://nodei.co/npm/vue-scroll/)

## Installation
### NPM(recommended)
```
npm install vue-scroll --save
```
### Standlone

Simple download from [releases](https://github.com/wangpin34/vue-scroll/releases) and include it in script tag.

## Usage
It's very simple, just declar in html tags and provide a defined callback - the scroll function below.

In javasript:
```javascript
new Vue({
  el: '#app',
  data: {},
  methods:{
    onScroll:function(e, position){
      this.position = position;
    }
  }
})
```

The function onScroll has two arguments, e is the scroll event object, position is an object which has two properties about the postion of scroll bar:
* scrollTop type:number
* scrollLeft type:number

In html:
```
<body v-scroll="onScroll">
...
</body>

```



## Samples

* Sample - commonjs [Introduction](https://github.com/wangpin34/vue-scroll/tree/2.0-compatible/samples/commonjs)
* [Sample - standlone](https://github.com/wangpin34/vue-scroll/tree/2.0-compatible/samples/standlone) *** [Try in now](http://rawgit.com/wangpin34/vue-scroll/2.0-compatible/samples/standlone/index.html)


## LICENSE
MIT
