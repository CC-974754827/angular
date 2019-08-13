# angular

```
<script src="https://cdn.staticfile.org/angular.js/1.4.6/angular.min.js"></script>
```

## 五个常用特性:
```
*ngFor
*ngIf
插值表达式 {{}}
属性绑定 []
事件绑定 ()
```
```
<h2>Products</h2>

<div *ngFor="let product of products">

  <h3>
    <a [title]="product.name + ' details'">
      {{ product.name }}
    </a>
  </h3>

  <p *ngIf="product.description">
    Description: {{ product.description }}
  </p>

  <button (click)="share()">
    Share
  </button>

</div>
```
## 组件
```
组件包含三部分：
一个组件类，它用来处理数据和功能。
一个 HTML 模板，它决定了用户的呈现方式。
组件专属的样式定义了外观和感觉。
```
每个内容有例子
