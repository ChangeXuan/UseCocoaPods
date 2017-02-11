# UseCocoaPods
## 网上已经有比较多的教程，只是有几点可能需要注意的东西
- 淘宝的镜像已经停止维护，现在使用'gem sources -a https://gems.ruby-china.org/' 新的镜像地址
- 配置好gem后执行pod setup用来初始化

## 不习惯vim的可以这样操作配置Podfile文件
- cd到工程目录，然后在终端内输入touch Podfile   //在工程目录中创建一个Podfile文件
- 双击打开Podfile然后编辑

## 使用swift的工程使用cocoaPods
- 在Podfile文件中添加一下文本
```
platform:ios,'9.0'
use_frameworks!

target 'pjName' do
pod 'Alamofire','~> 4.0'
end
```

- 然后在终端内输入 pod install

## 直接使用import xxx 就可以导入了
