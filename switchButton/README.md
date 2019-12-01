### 知识点       

1. CSS——相邻兄弟选择器 ” + “，选择紧接在另一个元素后的元素，且二者有相同的父元素。注意：选择是是一个元素，也就是符合条件的兄弟元素     

```css
input:checked + .circle{...}
```

如上，选择的是input:checked的兄弟元素，类名为.circle     

2. label标签。label标签的主要作用是扩大元素的鼠标捕捉范围，也就是点击的面积。label标签本身不会呈现任何特殊效果。label标签常与表单标签如input、form一起使用。labe标签的for属性绑定的是关联元素的id,这是**显示关联**，或者将关联元素写在label标签内，也就是**隐式关联**。    

```html
<!--显示关联-->
<form>
  <input type='text' name='username' id='username' />
  <input type='password' name='password' id='password' />
</form>
<label for='username'>用户名</label>
<label for='password'>密码</label>

<!--隐式关联-->
<form>
  <label>
    <input type='text' name='username' id='username' />
    用户名
  </label>
  <label>
    <input type='password' name='password' id='password' />
    密码
  </label>
</form>
```

