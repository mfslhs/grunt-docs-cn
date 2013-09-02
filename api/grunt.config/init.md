# grunt.config.init()

初始化配置。

### .init(config)

* `config` Object
* 返回值 Object

`config` 可通过 `grunt.config()` 访问：

    grunt.config.init({
        name: 'gruntjs.cn'
    });
    //调用 grunt.config() 输出：{ name: 'gruntjs.cn'}

配置中可包含 `<% %>` 模板字符串：

    grunt.config.init({
        host: 'gruntjs.cn',
        name: '<%= host %>'
    });
    //调用 grunt.config() 输出：{ host: 'gruntjs.cn', name: 'gruntjs.cn'}

[http://gruntjs.cn/api/config.init/](http://gruntjs.cn/api/config.init/)