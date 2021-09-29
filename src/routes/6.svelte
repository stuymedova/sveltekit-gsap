<script>
  import { onMount } from 'svelte'
  import { gsap } from 'gsap'

  let container
  
  onMount(() => {
    gsap.fromTo(
      container.children, 
      { opacity: 0 },
      { opacity: 1, stagger: 0.1, ease: 'expo' })
  })
</script>


<div bind:this={container} id='container'>
  <div class='element'></div>
  <div class='element'></div>
  <div class='element'></div>
  <div class='element'></div>
</div>


<style>
  #container {
    display: flex;
  }

  .element {
    height: 150px;
    width: 150px;
    margin: 1rem;
    padding: 0;

    position: relative;
    opacity: 0;
    background-color: #00bb00;
  }
</style>