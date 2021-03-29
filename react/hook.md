### Hook

- Hook 是一些可以让你在函数组件里钩入 React State 及生命周期等特性的函数

* Hook 使用规则
  - 只能在函数最外层调用 Hook，不能再循环，判断中判断
  - 只能再 react 的函数组件中调用 Hook

- useState()
  - useState() 在组件第一次执行时创建，之后值只能通过 SetCount 函数改变
  * `const [count,setCount]=useState(0)`返回值
    - count 是 useState 声明的 state 变量，
    * setCount 是更新 state 的函数
  - useState 可以在组件中多次调用
  * `setCount(count+1)` +`you click ${count} times` 模板字符串中`${count}`使用 state 变量

* useEffect()副作用函数
  - 告诉 react 组件需要在渲染后执行某些操作
  * 是 componentDidMount，componentDidUpdate 和 componentWillUnmount 这三个函数的组合
  - 在组件初始化，更新时调用
  * useEffect()可以返回一个清除函数，在组件每次渲染时都会执行

- useCallback
- 返回一个 memoized 函数，`const memoizedCallback = useCallback(()=>{dosomeing(a,b);},[a,b],)`
  - 接收两个参数，第一个回调函数，第二个回调函数依赖项数组
