# grunt.config.get()

获取项目配置对象或其中一个配置的值。

### .get([prop])

* `prop` String - 配置的键
* 返回值 Object

当没有传入 `prop` 时，获取整个项目配置对象：

    //grunt.config.init({ name: 'gruntjs.cn' });
    grunt.config.get(); //{ name : 'gruntjs.cn' }

当传入 `prop` 时，获取一个配置的值：

    grunt.config.get('name'); //gruntjs.cn

`<% %>` 模板字符串会自动调用 `grunt.config.process()` 处理：

    //grunt.config.init({ project: 'gruntjs.cn', name: '<%= project %>' });
    grunt.config.get('name'); //gruntjs.cn

[http://gruntjs.cn/api/config.get/](http://gruntjs.cn/api/config.get/)