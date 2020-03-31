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

合法提交案例

``````javascript
<!DOCTYPE html>
<html>
<head>
    <meta charset="UTF-8"/>
    <script type="text/javascript">
        function onsubfun(){
            var usenameobj = document.getElementById("xm");
            var usenametext = usenameobj.value
            var patt = /^\w{5,12}$/;//允许数字，字母，下划线5~12位
            if(patt.test(usenametext)){
                alert("合法");
                return true;
            }
            else{
                alert("不合法");
               return false;
            }
        }
    </script>
    
</head>

    <body>
        <form action="http://localhost:8080/" method="GET" onsubmit="return onsubfun();">
            姓名<input type="text" id="xm" value="kongbai"/><br/>
            密码<input type="password" id="mm"/>
            提交1<input type="submit" />
        </form>

    </body>

</html>
``````

正则表达式

``````javascript
var patt = / /;//正则表达式标准格式
var patt2 = /e/;//字符串是否含有e 
var patt3 = /[asb]/;//字符串是否含有e 
var patt4 = /[a-z]/;//字符串是否含有abcde...z
var patt5 = /[\w]/;//字符串是否含有字母数字下划线
var patt6 = /a+/;//字符串中包含含有一个a 
var patt7 = /a*/;//字符串是否包含有0个或者多个 
var patt8 = /a？/;//字符串是否包含有0个或者1个 
var patt9 = /a{3}/;//字符串是否至少包含连续3个a 
var patt9 = /a{3,5}/;//字符串是否至少包含连续3个a，最多5个a 
var patt9 = /a$/;//字符串是以a结尾
var patt9 = /a^/;//字符串是否以a开头 
var patt9 = /^a{3,5}$/;//字符串是否从头到尾至少三个最多五个a 
``````



