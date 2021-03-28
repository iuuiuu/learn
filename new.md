+ `const uuidv4 = require('uuid/v4')`,`uuidv4()` 方法用于生成一个理论上不重复的128位16进制的代码
+ `navigator.userAgent` 声明了浏览器用于 HTTP 请求的用户代理头的值
+ `numberObject.toFixed(num)`,`num.toFixed(1)`  把num四舍五入为1位小数的数字
+ process是node中表示当前node进程的全局变量
     + `if(process.browser)`判断是否为客户端
     + `process.env`包含着关于系统环境的信息
        + `process.env.NODE_ENV`用户自定义变量，用来判断当前是开发环境还是生产环境
+ ??判断符号
    + `process.env.NODE_ENV ?? 'development'`,判断问号前值是否为空，为空赋予后面的值，不为空跳过，取原来变量值