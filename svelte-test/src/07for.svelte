<script>
    let name = '과일'
    let fruits = ['사과','바나나','키위','포도','딸기']
    function deleteFruit(){
        fruits = fruits.slice(1)
    }
</script>
<h1>Hello {name}</h1>
<ul>
    <!-- fruits배열의 요소들을 fruit라는 name으로 each 돌림 -->
    {#each fruits as fruit}
       <li>{fruit}</li> 
    {/each}
</ul>
<button on:click={deleteFruit}>
    Eat it!
</button>