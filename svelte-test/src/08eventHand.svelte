<script>
    // import {onMount} from 'svelte'
    let name = 'world'
    let isRed = false
    // onMount(()=>{
    //     const box = document.querySelector('.box')
    //     box.addEventListener('click', () => {isRed = !isRed})
    // })
    function enter() {
        name = 'enter'
    }
    function leave() {
        name = 'leave'
    }
</script>

<h1>Hello {name}!</h1>
<div class = "box"
    style="background-color: {isRed ? 'red' : 'orange'};"
    on:click={() => {isRed = !isRed}}
    on:mouseenter={() => {name = 'enter'}}
    on:mouseleave={() => {name = 'leave'}}>	Box!</div>
    <!-- on 디렉티브는 이벤트리스너의 모든것에 사용가능하다. 
    위의 방식은 아래처럼 동일하게도 사용이 가능하다.
        on:click={() => {isRed = !isRed}}
        on:mouseenter={enter}
        on:mouseleave={leave}>	Box!</div>

-->
<style>
    .box{
        width: 300px;
        height: 150px;
        background-color: orange
    }    
</style>