# grunt.config.init()

为当前项目初始化一个配置对象，同 `grunt.initConfig()`。

## .init(config)

* `config` Object
* 返回值 Object

`config` 可通过 `grunt.config()` 访问：

    grunt.config.init({
        name: 'gruntjs.cn'
    });
    //调用 grunt.config() 输出：{ name: 'gruntjs.cn'}

当配置数据被获取时，`<% %>` 模板字符串会被执行：

    grunt.config.init({
        host: 'gruntjs.cn',
        name: '<%= host %>'
    });
    //调用 grunt.config() 输出：{ host: 'gruntjs.cn', name: 'gruntjs.cn'}
