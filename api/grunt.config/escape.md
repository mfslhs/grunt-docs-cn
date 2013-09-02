# grunt.config.escape()

转换带点号的配置属性名。

### .escape(str)

* `str` String - 配置属性名
* 返回值 String

当配置属性名中包含 `.` 点号时调用该方法进行转换：

    //grunt.config.init({ 'a.b' : 'gruntjs.cn'});
    //grunt.config.get('a.b'); //undefined
    grunt.config.escape('a.b'); //
    //grunt.config.get( grunt.config.escape('a.b') ); //'gruntjs.cn'

[http://gruntjs.cn/api/config.escape/](http://gruntjs.cn/api/config.escape/)