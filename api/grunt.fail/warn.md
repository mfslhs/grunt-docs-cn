# grunt.fail.warn()

抛出警告。

### .warn(error [, errorcode])

* `error` String | Object - 错误信息
* `errorcode` Number - 错误代码
* 返回值 Void

抛出警告，程序终止；也可以运行 `grunt --force` 忽略警告使程序不中断：

    grunt.registerTask('default', '', function(){
        grunt.fail.warn('errorStr');
    });
    //运行 grunt
    //Running "default" task
    //Warning: errorStr

[http://gruntjs.cn/api/fail.warn/](http://gruntjs.cn/api/fail.warn/)