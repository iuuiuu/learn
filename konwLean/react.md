### react 基本使用方法

- 在 react 中，父组件向子组件传参数在父组件的子组件标签中，使用属性向子组件传值，<child value={i} />,在子组件中，使用 props 接收这个值，以{this.props.value}使用传入的参数

* 在组件中的构造函数中，必须以 super(props)开头，"this.state={value:null}"存放数据，在方法中以 this.setState({value:"X"})来修改 state 中的值

### 状态提升

- 将子组件的 state 数据传递给父组件，父组件通过 props 在将在数据传递给子组件，实现状态数据共享

* 在父组件中调用子组件时，可以向子组件传递方法参数'child value={i} onClick={function()}',在子组件中通过{this.props.onClick()}调用该函数

### 自定义组件在传递方法为参数时，方法课以自定义名称

### this.setState() 方法用于修改 state 中的值

## react 知识点

- npx create-react-app my-app 创建一个新的 react 项目

* 一个 jsx 标签内没有内容，可以使用/来闭合<squares />
