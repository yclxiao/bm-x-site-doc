# bm-x-site-doc关于建站的流程简单说明

## *建站部件*

```
x-site-server
x-site-client
x-site-opapi
x-site-roach
x-site-render
x-site-tpl-dev
x-site-tpl-manager
x-site-ui
```

## *大致说明*

```
1. x-site-server + x-site-client + x-site-openapi是看到的可以编辑的页面
2. 点击发布，利用x-site-roach将编辑的组件组合成html存放到了aliyun
3. 各个业务线调用x-site提供的接口，到aliyun的oss上获取html页面
```


## *问题说明*

#### 1、模板 x-site-ui-home
window.xSiteIntegrate  此对象

__XSite_widgetInject

模板的组件分为  qmBar     qmGroup


#### 2、主要信息存放位置

用户编辑的模板对应的数据在库里pageinfos

对应的生成的文件位置在：http://bm-oss.oss-cn-hangzhou.aliyuncs.com/x-site/test/public/barRepo/x-site-ui-ehome，x-site-ui-ehome：代表每个业务线的工程名字

[某个用户编辑的内容](./pageinfos)


#### 3、[这段js作用](https://bm-oss.oss-cn-hangzhou.aliyuncs.com/x-site/test/public/buildTemplate/ehome-index-demo3.js)

```
https://bm-oss.oss-cn-hangzhou.aliyuncs.com/x-site/test/public/buildTemplate/ehome-index-demo3.js
```
	
#### 4、x-site-server  的 这个链接  /mysite/pc/index/1505979404711  做了啥？
![](./images/4-1.png)

#### 5、看看这里做了啥/Users/yclxiao/Project/bm-x-site/packages/x-site-web-client/assets/apps/prototype  的js渲染的啥？再看看这个编辑页面怎么把模板渲染出来的？

#### 6、发布时，保存哪些东西？到了小强之后，小强怎么组装页面。

#### 7、小强是如何获取任务，渲染页面的？

#### 8、html放在哪个路径，render怎么取页面

#### 9、window下挂载了哪些对象？什么部件往window里挂对象了？






