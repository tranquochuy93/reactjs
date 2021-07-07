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
