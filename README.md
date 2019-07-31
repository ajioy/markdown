[TOC]


## 标题
大标题，放在===上面
===
中标题，放在---上面
---
# 一级标题H1
## 二级标题H2
### 三级标题H3
#### 四级标题H4
##### 五级标题H5
###### 六级标题，不能再小了H6

---
## 正文
正文，常规文本，不需要任何标识。回车键不能直接换行，只能用以下两种方式。
1. 两个空格+回车
2. 用\< br>或\< br\/>

这是个用例，我要换行了。  
成功换行。
另一种方式换行。<br>
也成功了。

---
## 强调
**两个\*加粗**   
__两个\_加粗__   
*一个星号斜体*  
_一个下划线斜体_  
~~两个\~删除线~~  
***三个星号是粗斜体***  
<u>下划线</u>  
这是`高亮显示`  
上标：X<sub>2</sub>，下标：O<sup>2</sup>  

        hello, i am ajioy! a Tab in head (8 space in head)
        something important here 

---
## 引用
> \>块引用  
> 换行内容  
> * 可以加列表

嵌套引用
> 外层引用
>> `内层`引用  
>> 还可以嵌套**加粗**，*斜体*等  
>>> 第三级引用
>>>> 第四级引用

---
## 列表  
### 无序列表 
* c++
- python
+ javascript

### 有序列表
1. apple
2. orange
3. banana

### 嵌套列表
* first
  * second
    1. third
    2. third another
* another one
  * great
    * fantastic

### 任务待办
- [x] 跑步
- [x] 买日常用品
- [ ] 数据备份
- [ ] 买菜做饭
---

## 排版
### 空格
* 不断行的空格 &nbsp; 或 &#160; 1/4 中文<br>
* 半角的空格 &ensp; 或 &#8194; 半个中文，1字符<br>
* 全角的空格 &emsp; 或 &#8195; 1个中文，2字符<br/>

### 分割符
三个减号，三个星号，三个下划线

---

***
___

### 对齐
<p align="left">left</p>  
<p align="center">center</p>  
<p align="right">right</p>  

### 字体
<font face="黑体">我是黑体字</font>  
<font face="微软雅黑">我是微软雅黑</font>  
<font face="STCAIYUN">我是华文彩云</font>  
<font color=#0099ff size=7 face="黑体">color=#0099ff size=72 face="黑体"</font>  
<font color=#00ffff size=72>color=#00ffff</font>  
<font color=gray size=72>color=gray</font>  
> Size：规定文本的尺寸大小。可能的值：从 1 到 7 的数字。浏览器默认值是 3

### 特殊符号
\\
\*
\_
\#
\+
\-
\.
\!<br>
&#10084;  
&#10003;  

&copy; &  &uml; &trade; &iexcl; &pound;
&amp; &lt; &gt; &yen; &euro; &reg; &plusmn; &para; &sect; &brvbar; &macr; &laquo; &middot;

X&sup2; Y&sup3; &frac34; &frac14;  &times;  &divide;   &raquo;

18&ordm;C  &quot;  &apos;


[more unicode symbols](https://unicode-table.com/cn/)

### emoji
[github emoji](https://www.webfx.com/tools/emoji-cheat-sheet/)

---
## 图片
### 普通图片
![pic](https://profile.csdnimg.cn/6/3/D/1_ajioy "my pic")

### 带链接的图片（方法一）
[![pic](https://profile.csdnimg.cn/6/3/D/1_ajioy "my pic")](https://blog.csdn.net/ajioy)

### 带链接的图片（方法二）
[![blog]](https://blog.csdn.net/ajioy)
[blog]:https://profile.csdnimg.cn/6/3/D/1_ajioy "my pic"

### 控制图片大小及对齐方式
* 方法一，平台通用的标签法
```html
<div align="right">
<img src="https://profile.csdnimg.cn/6/3/D/1_ajioy" width="400px" height="300px">
<img src="https://profile.csdnimg.cn/6/3/D/1_ajioy" width="400px" height="300px">
</div>
```
<div align="right">
<img src="https://profile.csdnimg.cn/6/3/D/1_ajioy" width="400px" height="300px">
</div>

* 方法二，部分平台支持
\!\[pic\]\(url\)，其中url后面加个空格，再=WIDTHxHEIGHT，HEIGHT可以省略。  
如 (http://url.jpg =400x300)
```markdown
![pic](https://profile.csdnimg.cn/6/3/D/1_ajioy =400x300)
![pic](https://profile.csdnimg.cn/6/3/D/1_ajioy =400x)
```


* 方法三，简书等部分平台支持  

\!\[pic\]\(url\)的基础上加上{:height="300px" width="300px"}

### 内部引用图片
todo

---
## 链接
直接链接1 https://blog.csdn.net/ajioy  
直接链接2 <https://blog.csdn.net/ajioy>  
[带标题链接](https://github.com/ajioy)  
[带标题链接且鼠标悬停](https://blog.csdn.net/ajioy "go to my blog")
---

## 表格
| 表头 | 名字 | 分数 |
|-:| :-: | :- |
| 101 | ajioy | 99.82 |
| 102 | scotte | 98.12 |
| 103 | bot | 97.23 |
> :--- 左对齐，冒号在左边  
> ---: 右对齐，冒号在右边  
> :--: 居中对齐，冒号两边  

---

## 代码
```python
def add(a, b):      // python
    return a + b
```

```bash
sudo apt-get install autojump # bash
```

```cpp
int main()
{
    printf("hello,ajioy"); // cpp
}
```

### diff
```diff
+ add
- delete
~ modify?
! what's this
# i don't known
```

---

## 脚注
### 方法一
句中作脚注，解释一个名词[^1]，再解释一个[^2]。  
脚注放在文章最下面，脚注可以直接放链接。
[^1]: 解释名词1  
[^2]: https://www.google.com 
### 方法二
整个句子作脚注。^[这里就是脚注内容，默认会生成脚注序号]  
`有道云`支持，不知道`github`和`evernote`是否支持。

---

## 视频
以B站为例，点分享按钮，复制`嵌入代码`，粘贴到md文件即可，其他网站类似。
<iframe src="//player.bilibili.com/player.html?aid=57373164&cid=100164001&page=1" width="600" height="300" scrolling="no" border="0" frameborder="no" framespacing="0" allowfullscreen="true"> </iframe>

---

## 地图

以百度地图为例，
访问API自定义地图 http://api.map.baidu.com/lbsapi/creatmap/index.html 

设置好地点、文字、路线、标记后，点获取代码，复制代码，直接放在md文件，或将代码存放在map.html文件，同一目录下，再引入markdown

---

## LaTeX公式
todo  
访问 [MathJax](http://meta.math.stackexchange.com/questions/5020/mathjax-basic-tutorial-and-quick-reference)

---

## 流程图
todo  
语法参考：[流程图语法参考](http://adrai.github.io/flowchart.js/)

---

## 序列图
todo  
语法参考：[序列图语法参考](http://bramp.github.io/js-sequence-diagrams/)

---

## 甘特图
todo  
语法参考：[甘特图语法参考](https://knsv.github.io/mermaid/#gant-diagrams)

---







## 最后是脚注的解释内容
[^1]:pumas are large cat-like animals which are found in America.  
[^2]:ruby is a script lanuage;


---
