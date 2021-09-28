<script>
  import { onMount } from 'svelte'
  import { gsap } from 'gsap'
  import { ScrollTrigger } from 'gsap/dist/ScrollTrigger';
  gsap.registerPlugin(ScrollTrigger);
  
  onMount(() => {
    gsap.to(
      '#element',
      { rotate: 360, ease: 'none',
        scrollTrigger: { trigger: '#wrapper', pin: true, scrub: true, markers: true }})
  })
</script>

<div id='wrapper'>
  <div id='element'></div>
</div>

<style>
  :global(body) {
    width: 100%;
    height: 100%;
    margin: 0;
    padding: 0;
    overflow: hidden;
  }
  
  #wrapper {
    height: 100vh;
    margin: 0;
    padding: 0;
  }
  #element {
    display: block;
    height: 150px;
    width: 150px;
    margin: 0;
    padding: 0;

    position: fixed;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    background-color: #00bb00;
  }
</style>