<script>
  import { onMount } from 'svelte'
  import { gsap } from 'gsap'
  
  onMount(() => {
    gsap.to(
      '#element', 
      { rotate: gsap.utils.random(-360, 360) })
  })
</script>

<div id='element'></div>

<style>
  #element {
    display: block;
    height: 150px;
    width: 150px;
    margin: 1rem;
    padding: 0;

    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    background-color: #00bb00;
  }
</style>