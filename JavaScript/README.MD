### 1.点击按钮弹出对话框  
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Title</title>
</head>
<body>

<!--版本1-->
<input type="button" value="1显示效果" onclick="alert('我被点了')"/>

<!--版本2-->
<script>
    function f1(){
        alert("这是一个对话框");
    }
</script>
<input type="button" value="2显示效果" onclick="f1()"/>

<!--版本3-->
<input type="button" value="3开始分离代码" id="btn"/>
<script>
    function f2() {
        alert("开始分离HTML和js代码");
    }
    var btnObj = document.getElementById("btn");
    btnObj.onclick = f2;//不加括号

</script>
<input type="button" value="显示效果" id="btn"/>

</body>
</html>
```
