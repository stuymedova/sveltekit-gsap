<script>
  import { onMount } from 'svelte'
  import { gsap } from 'gsap'
  
  onMount(() => {
    gsap.fromTo(
      '.element', 
      { opacity: 0 },
      { opacity: 1, stagger: 0.1, ease: 'expo' })
  })
</script>

<div id='wrapper'>
  <div class='element'></div>
  <div class='element'></div>
  <div class='element'></div>
  <div class='element'></div>
</div>

<style>
  :global(#wrapper) {
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