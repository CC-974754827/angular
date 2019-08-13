AngularJS 通过新的属性和表达式扩展了 HTML。

AngularJS 可以构建一个单一页面应用程序（SPAs：Single Page Applications）。
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
使用 ng-include 指令来包含 HTML 内容

动画
```
<script src="http://cdn.static.runoob.com/libs/angular.js/1.4.6/angular-animate.min.js"></script>
```
依赖注入
```
value  是一个简单的 javascript 对象，用于向控制器传递值。（配置阶段）
factory 是一个函数用于返回值。在 service 和 controller 需要时创建。
service
provider 中提供了一个 factory 方法 get()，它用于返回 value/service/factory。
constant (常量)用来在配置阶段传递数值，注意这个常量在配置阶段是不可用的。
```
路由
```
<script src="https://cdn.bootcss.com/angular.js/1.7.0/angular-route.min.js"></script>
```
