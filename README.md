#工具

工具组件包含开发中常用的一些小功能。

[TOC]

####创建实例对象
```
$obj = new \houdunwang\tool\Tool();
```

####生成随机数
```
//生成10位随机数
$obj->rand(10);
```

####批量执行函数

```
$funcs=['md5','strtoupper'];
$value='houdunwang';
$obj->batchFunctions($funcs,$value);
//一个函数时的执行
$obj->batchFunctions('md5','hdphp');
```

####可识别的单位
根据大小返回标准单位 KB  MB GB等
```
$obj->getSize(20000,2);
//计算20000是GB还是MB，并返回2位小数
```