# grunt.config.getRaw()

获取配置，但不处理模板字符串。

### .getRaw([prop])

* `prop` String - 配置的键
* 返回值 Object

例子：

    //grunt.config.init({ project: 'gruntjs.cn', name: '<%= project %>' });
    grunt.config.getRaw('name'); //<%= project %>

[http://gruntjs.cn/api/config.getRaw/](http://gruntjs.cn/api/config.getRaw/)