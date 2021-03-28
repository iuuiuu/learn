### TS
+ 给函数的参数添加类型注解
    + `function hello(name: string){}`，约束传入的参数是字符串类型
+ `interface Person{}`定义一个接口，约束参数数组的属性
### TS数据类型除了JS常有的之外，还有一些扩展
+ any,当不清楚变量类型的时候，使用any通过编译阶段的检查
    + any类型的变量在定义时可以使用方法，表示可能会发生
    + void表示没有任何类型，当一个函数没有返回值时
    + object表示非原始类型，如对象，但不访问任何键
    + `Record<any, any>`，允许访问任何键
### 接口就是定义一个类型，对参数变量进行约束
+ `interface Person{name :string }`要求传入的参数的name属性必须是字符串类型
+ 可选属性`interface Person{name?:string}`name属性存在与否是可选择的，可传可不传
+ 只读属性 `interface Point{readonly x:number}`定义了只读属性的变量值不能被修改
+ 函数接口，
    + `interface FunctionName{(name:string,age:number):boolean}`，第一个参数定义函数接受参数的属性类型，第二个参数指定函数返回值的类型
    + `interface Myfunc{ function1:(name:string)=>void}`
        + ()指定参数是函数，箭头指定参数返回值时void
### 类型断言，清楚的知道一个实体更确切的类型，两种方式
+ 尖括号，<any>该变量的值类型是any
+ as ,`somevalue as string `某个值类型是string
### 模块
+ 模块导出
    + 任何声明都能通过export关键字导出，`export interface MyInterface`
+ 模块导入 
    + `import {MyInterface} from 'interface'`
