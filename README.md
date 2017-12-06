# 埃文官网

创作不易，大神轻喷，如需源码，联系本人

## 代码概要

```js
Lorem ipsum dolor sit amet consectetur, adipisicing elit. Quidem minus distinctio veritatis 
perferendis neque repudiandae id expedita sint iusto, soluta quam officiis nobis autem 
quasi ipsum, nesciunt voluptate vero nam officia voluptatum? Sunt dolore, assumenda,
soluta itaque perferendis deleniti placeat nostrum, vitae nihil quia voluptatum tenetur 
nulla minus reiciendis libero eveniet iure voluptatem repellendus quisquam. Sapiente 
maiores rerum, eveniet nisi quas, inventore ipsam expedita perferendis sint possimus,
tempore at vitae laborum quos id enim ratione fugiat eius? Sunt hic fuga reprehenderit.
Minima ea aliquid, hic ducimus fugiat dolorum repellat ut doloremque nulla cupiditate 
odio illum a temporibus magni reprehenderit omnis!
```

## 网站总体设计

埃文官网共分为九个版块，实现了企业展示站的主要需求。设计风格简洁大方，主要以浅色调为主。下面是各个版块的详细介绍。

### 首页

埃文官网主页在结构上采用当前流行瀑布布局，由topBanner，nav，silder，mian，footer层层递进，但是不同于以往的网站设计，埃文官网首页的main部分直接写埃文核心产品的应用领域，产品优势和产品服务。

### 产品中心

埃文当前的产品为IP问问-高精准，IP问问-区县级和IP应用场景（IP Scene）三大系列。三大系列产品的结构相同，都是nav+items。

* IP问问-高精准

IP问问-高精准从定位原理，综合服务，产品优势，应用领域和测试方法五大方面进行阐述,其中定位原理中的定位精度说明采用slider。[更多设计细节](https://github.com/redliyang/ipplus360)

* IP问问-区县级

IP问问-高精准从服务能力，产品优势，应用领域，测试方法和常见问题五大方面进行阐述。[更多设计细节](https://github.com/redliyang/ipplus360)

* IP应用场景（IP Scene）

IP应用场景（IP Scene）从场景分类说明，产品综合服务能力，产品优势和应用领域四大方面进行阐述。[更多设计细节](https://github.com/redliyang/ipplus360)

### 应用领域

### 技术支持

### 公司介绍

### 实用工具

### 客户专区

### 帮助与支持

### 商城

## 工作流

### JDF

前段自动化工具有很多，有老生常谈的Gulp/Grunt/Webpack，虽然自己配置非常有成就感，而且方便装X，如果项目赶得比较紧的话，恐怕都没有配置的乐趣了。所以每一个前端工程师都需要一套完整的自动化和工程化解决方案。比如京东的JDF，简单，好用。

JDF官方简介[点此了解更多](https://github.com/putaoshu/jdf)

* JDF京东前端开发集成解决方案，（Jingdong front-end integrated solution）
* 目的是合理、快速和高效的解决前端开发中的工程和项目问题，主要提供了：
* 前端命令行工具：集调试、构建、布署为一体
* 前端模块：下载、预览、发布
* 前端开发流程：项目构建、编译、输出、联调、上线
* 前端组件：UI组件和业务组件（内网开源）
* 前端文档：编码规范、开发规范、组件和工具文档
* 前端周边扩展：代码文档和示例自动生成工具、代码编辑器插件、可视化工具等

### 姓氏命名法

当项目非常大的时候，我想每个前段工程师都会对庞大复杂的CSS感到头疼，如果是多人开发的话，每个人的CSS命名方式都不会太一样，所以当改需求看别人写的CSS的时候，绝对是一场噩梦。由此，CSS的BEM命名法应运而生，虽然BEM很流行，且褒贬不一，但是我用的是BEM的简化版本--姓氏命名法。

下面是姓氏命名法的简介，[点此了解更多](https://www.zhihu.com/question/54962942)

核心，只要保证最外层模块名不重复，模块内部可以任意命名。

* 简单模块：在子孙模块数量可预测的情况下，继承祖先模块的命名前缀

如:

```css
slider
├── slider-list
|    |
|    └── ....
└── slider-nav
|    |
|    └── ....
```

* 复杂模块：当子孙模块数量较多，且无法预估时，可以选择采用继承“祖先+父”模块的命名前缀，以保证模块之间的独立性

如：

```css
floor
├── floor-hd
|    |
|    ├── floor-tit
|
├── floor-item
|    |
|    ├── floor-item-tit
|    └── floor-item-desc
```

* 复合模块：子模块中，可以嵌套其他模块，可理解为“娶媳妇”

如：

```css
hotsales
├── hotsales_li
| |
| └── mod_goods
| |
| ├── mod_goods_price
| └── mod_goods_tit
| └── mod_goods_promo
```