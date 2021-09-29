<script>
  // Using GSAP with Svelte:
  // https://stackoverflow.com/questions/62780343/

  import { onMount } from 'svelte'
  import { gsap } from 'gsap'
  
  let element

  onMount(() => {
    gsap.to(
      element, 
      { x: 400 })
  })
</script>


<div bind:this={element} id='element'></div>


<style>
  #element {
    display: block;
    height: 150px;
    width: 150px;
    margin: 1rem;
    padding: 0;

    position: absolute;
    top: 0;
    left: 0;
    background-color: #00bb00;
  }
</style>