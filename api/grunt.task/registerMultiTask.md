# grunt.task.registerMultiTask()

注册多重任务。

### .registerMultiTask(taskName, description, taskFunction)

* `taskName` String - 任务名
* `description` String - 任务描述
* `taskFunction` Function - 任务函数
* 返回值 Void

例子：

    grunt.config.init({
        default: { a: 1, b: 2 }
    });
    grunt.task.registerMultiTask('default', '', function() {
        console.log(this.data);
    });
    //运行 grunt
    //Running "default:a" (default) task
    //1
    //Running "default:b" (default) task
    //2

[http://gruntjs.cn/api/task.registerMultiTask/](http://gruntjs.cn/api/task.registerMultiTask/)