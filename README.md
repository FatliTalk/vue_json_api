# vue_json_api
Vue-使用JSON和AJAX传递API数据。还有vuejs数据驱动界面（可输入字数提醒），删除评论、修改字体大小、弹框功能

<br>
<br>
<br>


## 一、实现vue数据驱动界面等功能

> 实现vuejs数据驱动界面（可输入字数提醒），删除评论、修改字体大小、弹框功能（[Animate.css](https://daneden.github.io/animate.css/)弹框效果：bounce）。

https://fatlitalk.github.io/vue_json_api/index-old.html

<br>

![实现vuejs数据驱动界面等功能](https://raw.githubusercontent.com/FatliTalk/vue_json_api/gh-pages/images/01.png)

<br>
<br>

---

<br>
<br>

## 二、Vue-使用JSON和AJAX传递API数据

> Vue-使用JSON和AJAX传递API数据：通过[Reqwest](https://github.com/ded/reqwest)库处理Ajax，动态获取swapi.co的API数据，而不是在页面中手动输入，输出静态页面。

https://fatlitalk.github.io/vue_json_api/

<br>

![Vue-使用JSON和AJAX传递API数据](https://raw.githubusercontent.com/FatliTalk/vue_json_api/gh-pages/images/03.png)

<br>
<br>

---

<br>
<br>


# 三、Vue-使用JSON和AJAX传递API数据+loading加载和filter过滤器

> Vue-使用JSON和AJAX传递API数据：过Reqwest库处理Ajax，动态获取swapi.co的API数据，而不是在页面中手动输入，输出静态页面。
> 增加Vue.js的computed计算属性：1.动态数据呈现：用Vue.js实现loading效果；2.已有资源的二次加工：filter过滤器效果。

https://fatlitalk.github.io/vue_json_api/index-new-loading&filter.html 

<br>

![Vue-使用JSON和AJAX传递API数据+loading&filter](https://github.com/FatliTalk/vue_json_api/blob/gh-pages/images/4-loading&filter.png?raw=true)

<br>
<br>

---

<br>
<br>

## 附：[Reqwest](https://github.com/ded/reqwest)：替代JQuery处理Ajax

```javascript
<script>
    // script标签中的内容复制到index.html文件到vue.js中的getData函数
    var a = {}
    // 在reqwest函数中传入JS对象
    reqwest({
        // 要请求哪个网址
        url:"https://swapi.co/api/people/1/",
        // 要请求的格式：html、xml、json、jsonp
        type:"json",
        // 请求的方法：默认是GET方法
        method:"get",
        // 要传递的参数：PATCH，POST和PUT请求。必须是查询String或JSON对象
        // data:{tag:"life"},
        // 如何处理取得的数据：请求成功完成时调用的函数
        success:function (resp) {
            // 把取得的数据放到变量a中
            a = resp
        }
    })
</script>
```

<br>

https://fatlitalk.github.io/vue_json_api/tryReqwest.html

<br>

![Reqwest：替代JQuery处理Ajax](https://raw.githubusercontent.com/FatliTalk/vue_json_api/gh-pages/images/02.png)
