# 默认模式下分包规则
- 默认模式只影响按需(on-demand)加载的代码块(chunk)，因为改变初始代码块会影响声明在HTML的script标签
- 新代码块可以被共享引用，OR这些模块都是来自node_modules文件夹里面
- 新代码块大于30kb（min+gziped之前的体积）
- 按需加载的代码块，最大数量应该小于或者等于5
- 初始加载的代码块，最大数量应该小于或等于3