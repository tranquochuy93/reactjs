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
