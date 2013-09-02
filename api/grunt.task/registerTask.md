# grunt.task.registerTask()

注册任务。

### .registerTask(taskName, description, taskFunction)

* `taskName` String - 任务名
* `description` String - 任务描述
* `taskFunction` Function - 任务函数
* 返回值 Object

### .registerTask(taskName, taskList)

* `taskName` String - 任务别名
* `taskList` Array[String] - 任务列表
* 返回值 Object

注册一个默认任务：

    grunt.task.registerTask('default', '', function(){});
    //运行 grunt
    //Running "default" task

注册一个名为 <code>gruntjs.cn</code> 的任务：

    grunt.task.registerTask('gruntjs.cn', '', function(){});
    //运行 grunt gruntjs.cn
    //Running "gruntjs.cn" task

注册一个带参数的任务，参数输入格式为 `taskName[:arg1][:arg2][:argN]`：

    grunt.registerTask('default', '', function(arg1, arg2){
        console.log('args', arg1, arg2);
    });
    //运行 grunt default:aaa:bbb
    //args aaa bbb

如果 `taskFunction` 返回 `false`，程序中断：

    grunt.task.registerTask('default', '', function(){
        return false;
    });
    //运行 grunt
    //Warning: Task "default" failed. Use --force to continue.

运行 `grunt --help` 会输出所有任务的 `taskName` 和 `description`：

    grunt.task.registerTask('default', 'defaultDesc', function(){});
    //运行 grunt --help
    //Available tasks
    //     default  defaultDesc

注册别名任务，当别名任务运行时，`taskList` 数组里的任务也会运行：

    grunt.task.registerTask('taskA', '', function(){});
    grunt.task.registerTask('taskB', '', function(){});
    grunt.task.registerTask('default', ['taskA', 'taskB']);
    //运行 grunt
    //Running "taskA" task
    //Running "taskB" task

[http://gruntjs.cn/api/task.registerTask/](http://gruntjs.cn/api/task.registerTask/)