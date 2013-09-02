# grunt.config.requires()

检查配置依赖。

### .requires(prop [, prop [, ...]])

* `prop` String - 配置的键
* 返回值 Void

当配置中对应的 `prop` 属性不存在或为 `null` 或为 `undefined` 时，程序终止：

    grunt.config.requires('gruntjs.cn');
    //Verifying property gruntjs.cn exists in config...ERROR
    //>> Unable to process task.
    //Warning: Required config property "gruntjs.cn" missing. Use --force to continue.

[http://gruntjs.cn/api/config.requires/](http://gruntjs.cn/api/config.requires/)