<script>
	let name = 'world';
	let age = 85
	// 반응성 확인
	setTimeout(()=> {
			name = 'RipJay'
			age = 36
	}, 3000)
</script>

<h1>Hello {name}!</h1>
<h2>
<!-- 선언적 렌더링이 가능함	 -->
	{age}
</h2>
<button>
	Assign
</button>