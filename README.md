### Life cycle
1. Mounting: Chỉ xảy ra 1 một khi component mount
- componentWillMount()
- render()
- componentDidMount(): nơi thực hiện các hàm AJAX, axios request, DOM hay update state

2. Updation
- componentWillReceiveProps(): đối với component con nhận từ cha, setState dùng trong hàm này
- shouldComponentUpdate(): tăng hiệu suất
- componentWillUpdate()
- componentWillMount()
- componentDidUpdate(): chạy animation

3. Unmount
- omponentWillUnmount
 ### Hook
#### 1. useState
#### 2. useEffect
 - useEffect Hook is combined by componentDidMount, componentDidUpdate, and componentWillUnmount .
 - What does useEffect do? call it later after performing the DOM updates.
 - Why is useEffect called inside a component? Placing useEffect inside the component lets us access the state variable (or any props) right from the effect.
 - Does useEffect run after every render? By default, it runs both after the first render and after every update
#### useContext and useReducer
- useContext : sharing state with multiple components
- useReducer : handling state by the state machine


### Redux
#### 1. Data flow
1. Data flow
- 1. store is the place we save the 1
- 2. getState is the method to get the state
- 3. action & reducer is the method to change the mapStateToProps
 - The action tell reducer what does it want to do. Then the reducer updates the state base on the type and additional data provided by action.

#### why should we use redux?
1. easy to share props between components and prevent prop-drilling
2. Using action and reducer to update the state can make it easier to control. 
 - The state can only be changed base on the actions we have defined. And all the logic about how the state should be changed is in the reducer
 - 
