# javaweb

动态注册：

``````javascript
//动态注册事件固定写法
window.onload = function(){
            alert("动态");
       
        
        // 动态注册的onclick事件
      /*获取标签对象document
        getElementById("id")
        注册事件
          */    
        var onclbj = document.getElementById("but");
        onclbj.onclick = function () {
            alert("动态onclick事件");
            }
        }
``````

