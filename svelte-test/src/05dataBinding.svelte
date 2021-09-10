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
<!-- class를 삼향연산자를 이용해서 유효성처리로 부여가 가능하다. WOW.. 이거 실화..? -->
<h2 class={age < 85 ? 'active' : ''}>
	{age}
</h2>
<img src="" alt={name} />
<br>
중괄호는 '선언적렌더링'을 시킨다 
<br>
<!--bind: 양방향-->
<!--단방향 <input type="text" value={name} >-->
<input type="text" bind:value={name} >

<button on:click = {assign}>
		Assign
</button>
<style>
	h1{
			color:red;
	}	
	.active{
		color:blue;
	}
</style>