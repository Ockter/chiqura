<script>
	let name = 'world';
	let toggle = false;
	if (toggle){
			
	}else{

	}
	// 	시작    구문  #
	//  끝나는  구문  /
	// 내용추가 구문  :

</script>
<!-- 버튼이벤트 시작시 변수의 값을 반전 -->
<button on:click={()=>{toggle  = !toggle}}>
	Toggle
</button>

<!-- {#if} : 시작 /	{/if} : 엔드 -->
{#if toggle}
<h1>Hello {name}!</h1>
{:else}
	<div>No name!</div>
{/if}