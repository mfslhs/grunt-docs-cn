# grunt.task.run()

运行任务。

### .run(taskName)

* `taskName` String - 任务名
* 返回值 Object

### .run(taskList)

* `taskList` Array[String] - 任务列表
* 返回值 Object

运行一个任务：

    grunt.registerTask('gruntjs.cn', '', function(){});
    grunt.registerTask('default', '', function(){
        grunt.task.run('gruntjs.cn');
    });
    //运行 grunt
    //Running "default" task
    //Running "gruntjs.cn" task

运行任务列表：

    grunt.registerTask('a', '', function(){});
    grunt.registerTask('b', '', function(){});
    grunt.registerTask('default', '', function(){
        grunt.task.run(['a', 'b']);
    });
    //运行 grunt
    //Running "default" task
    //Running "a" task
    //Running "b" task


[http://gruntjs.cn/api/task.run/](http://gruntjs.cn/api/task.run/)