<script>
	let name = 'world';
	let age = 85
	//반응성 확인 : 메서드
	function assign(){
		name = 'RipJOK'
		age = 36
	}
</script>

<h1>Hello {name}!</h1>
<h2>
<!-- 선언적 렌더링이 가능함	 -->
	{age}
</h2>
<!-- 이벤트 핸들링 방식 -->
<button on:click = {assign}>
		Assign
</button>