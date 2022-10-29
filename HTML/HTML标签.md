# HTML

Hyper Text Markup Language(超文本标记语言)

------

DOCTYPE:告诉浏览器我要使用什么规范

- 水平线标签：

```HTML
<hr>
```

- 粗体标签：

```HTML
<strong></strong>
```

- 斜体标签：

```HTML
<em></em>
```

- 符号：

```HTML
大于 &gt ; 小于 &lt ; 版权符号 &copy
```

- 图片标签：

```HTML
<img src="图片路径" alt="图片加载不出的提示" title="鼠标悬停时显示文字" width="" height="">
```

- 链接标签：

```HTML
<a href="网页链接" target=""></a>
```

- 锚点标签：

```HTML
<a id="top">顶部</a>
<a herf="#top">回到顶部</a>
可以页面见跳转
```

- 邮件标签：

```HTML
<a herf="mailto:加邮箱"></a>
QQ邮箱拥有推广自动创建
```

- 列表标签：

```HTML
有序列表 <ol>
		<li></li>
		</ol>
无序列表 <ul>
		<li></li>
		</ul>
自定义列表 <dl>
		 <dt>标题</dt>
		 <dd></dd>
		 </dl>
```

- 表格标签：

```HTML
行 <tr></tr>
列 <td colspan="合并的行数" rowspan="合并的列数"></td>
<table></table>
```

- 视屏标签：

```HTML
<video src="视频文件" controls控制条 autoplay自动播放></video>
```

- 音频标签：

```HTML
<audio 属性同上视频标签></audio>
```

- 页面结构标签：

```HTML
<header></header> 头部标签
<footer></footer> 脚部标签
<section></section> 独立区域标签
<article></article> 独立文章内容标签
<aside></aside> 相关内容或应用(常用于侧边栏)
<nav></nav> 导航类辅助标签
```

内联标签：

```HTML
<iframe src="地址" name="框架标识名(a标签跳转)" width="" height=""></iframe>
```

- 表单标签：

```HTML
<form method="post/get" action="表单提交的位置">
<p>用户名<input type="text" name="username"></p>
<p>密码<input type="password" name="pwd"></p>
<p><input type="submit" value="提交"></p>
<p><input type="reset" value="重填"></p>
</form>
```

- 文本框标签：

```HTML
<input pattern="正则表达式" placeholder="文本框提示信息" required非空></input>

文本框：<input type="text" name="username"/><br/>
密码框：<input type="password" name="password"/><br/>
隐藏域：<input type="hidden" name="userId" value="1001"/><br/>
多行文本域<br/>
留言：<textarea name="desc" rows="10" cols="50">默认值写在这里</textarea>
单选框<br/>
你最喜欢的季节是：
<input type="radio" name="season" value="spring" />春天
<input type="radio" name="season" value="summer" checked="checked" />夏天
<input type="radio" name="season" value="autumn" />秋天
<input type="radio" name="season" value="winter" />冬天 <br/>
多选框<br/>
你最喜欢的球队是：
<input type="checkbox" name="team" value="Brazil"/>巴西
<input type="checkbox" name="team" value="German" checked="checked"/>德国
<input type="checkbox" name="team" value="France"/>法国
<input type="checkbox" name="team" value="China" checked="checked"/>中国
<input type="checkbox" name="team" value="Italian"/>意大利<br/>
下拉框<br/>
你喜欢的运动是：
<select name="interesting">
<option value="swimming">游泳</option>
<option value="running">跑步</option>
<option value="shooting" selected="selected">射击</option>
<option value="skating">溜冰</option>
</select><br/>
按钮<br/>
<button type="button" value="普通按钮">普通按钮</button>
<button type="submit" value="提交按钮">提交按钮</button>
<button type="reset" value="重置按钮">重置按钮</button>
```

- 下拉框标签：

```HTML
<select name="列表名称" id="">
<option value=""></option>
</select>
```

- 文本域标签：

```HTML
<textarea name="" cols="列" rows="行"></textarea>
```
