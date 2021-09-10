<script>
	//data binding
	let name = 'world';
	let age = 85
	function assign(){
		name = 'RipJOK'
		age = 36
	}
</script>

<h1>Hello {name}!</h1>
<h2>
	{age}
</h2>
<img src="" alt={name} />
<br>
중괄호는 '선언적렌더링'을 시킨다 
<br>
<!--inpt의 value는 단방향 바인딩이기 때문에 변수에는 영향을 미치지 않는다. -->
<input type="text" value={name} >

<!-- 양방향 데이터 바인딩 : 버튼을 누르게되면 모든 변수의 data가 수정된다. -->
<button on:click = {assign}>
		Assign
</button>