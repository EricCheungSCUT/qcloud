## 简介
iOS模块化流程工具说明
```
gem install cocoapods-packager
gem install qscaffold

```
## 开发
Cocoapods 私有库
![](http://imagebad-1253653367.cosgz.myqcloud.com/Screen%20Shot%202018-07-11%20at%201.24.56%20PM.png)

通过 Cocoapods 集成私有库
```
pod 'TACCore', path:"~/Codes/TACCore"
pod 'QCloudCOSXML', path:"~/Codes/QCloudCOSXML"
```

## 打包
cocoapods-packager-qcloud
```
pod package TACCore.podspec
```
## 依赖问题
QScaffold

```
qscaffold module codeversion --rclt podspecs.rclt  -n all
```

## 发布
QScaffold
```
QSCaffold module publish -i podspecs.rclt -n TACCore
```

Shell 脚本：
事务，验证
