# Vue

声明式，响应式

## v-on:click=“方法”

``````html
<button v-on:click="substance()“</button>   
<!--语法糖-->
<button @click="substance()"></button>
``````

## v-once

``````html
 <h1 v-once>{{count}}</h1>
<!--不会在控制台被改变，该元素只会被渲染一次
	后面不接表达式
-->
``````

## v-html

``````html
 <h2 v-html="url"></h2>
<!-- 将标签渲染-->
url:'<a href="http://baidu.com">百度一下</a>'
``````

## v-pre

``````html
<h2 v-pre>{{message}}</h2>
<!--该标签不渲染-->
``````

## v-cloak

``````html
<div id="app" v-cloak>
    {{message}}
</div>
<!--当message未被解析之前，隐藏原码-->
``````

## v-bind

``````html
<img v-bind:src="imgURL",art=""/>
<!--通过解析指令，动态的绑定变量-->

<!--语法糖-->
<img :src="omgURL",art=""/>

<!--动态的给组件-->
<h2 v-bind:class:"{类名1:boolean，类名2:boolean}">{{message}}</h2>
``````



## let/const定义变量

``````html
<script>
            const app = new Vue({//const常量/let变量
                el:'#app',//通过id绑定组件
                data:{//定义数据
                    count:0
                },
                methods:{//定义方法
                    incream:function(){
                        this.count++;
                    },
                    substance:function(){
                        this.count--;
                    }
                }
            })
        </script>
``````



## 语法糖

语法简写

`````html
v-on:click//等价于@click
`````

