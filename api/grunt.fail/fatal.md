# grunt.fail.fatal()

抛出致命错误。

### .fatal(error [, errorcode])

* `error` String | Object - 错误信息
* `errorcode` Number - 错误代码
* 返回值 Void

抛出致命错误，程序终止：

    grunt.registerTask('default', '', function(){
        grunt.fail.fatal('errorStr');
    });
    //运行 grunt
    //Running "default" task
    //Fatal error: errorStr

[http://gruntjs.cn/api/fail.fatal/](http://gruntjs.cn/api/fail.fatal/)