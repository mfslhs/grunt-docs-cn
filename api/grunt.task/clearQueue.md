# grunt.task.clearQueue()

清除队列。

### .clearQueue()

* 返回值 Object

例子：

    grunt.registerTask('a', '', function(){
        grunt.task.clearQueue();
    });
    grunt.registerTask('b', '', function(){});
    grunt.registerTask('default', '', function(){
        grunt.task.run(['a', 'b']);
    });
    //运行 grunt
    //Running "default" task
    //Running "a" task

[http://gruntjs.cn/api/task.clearQueue/](http://gruntjs.cn/api/task.clearQueue/)