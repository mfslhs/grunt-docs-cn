# grunt.config.get()

获取配置。

### .get([prop])

* `prop` String - 配置的键
* 返回值 Object

获取全部配置：

    //grunt.config.init({ name: 'gruntjs.cn' });
    grunt.config.get(); //{ name : 'gruntjs.cn' }

获取一个配置：

    //grunt.config.init({ name: 'gruntjs.cn' });
    grunt.config.get('name'); //gruntjs.cn

获取带 `<% %>` 模板字符串的配置：

    //grunt.config.init({ project: 'gruntjs.cn', name: '<%= project %>' });
    grunt.config.get('name'); //gruntjs.cn

[http://gruntjs.cn/api/config.get/](http://gruntjs.cn/api/config.get/)