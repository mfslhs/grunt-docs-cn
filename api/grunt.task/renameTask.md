# grunt.task.renameTask()

重命名任务。

### .renameTask(oldname, newname)

* `oldname` String - 旧任务名
* `newname` String - 新任务名
* 返回值 Object

重命名后，旧任务名与原任务断开联系：

    grunt.registerTask('oldTask', '', function(){});
    grunt.task.renameTask('oldTask', 'newTask');
    //运行 grunt newTask
    //Running "newTask" task
    //运行 grunt oldTask
    //Warning: Task "oldTask" not found.



[http://gruntjs.cn/api/task.renameTask/](http://gruntjs.cn/api/task.renameTask/)