<script>
  import { onMount } from 'svelte'
  import { gsap } from 'gsap'
  import { SlowMo } from 'gsap/dist/EasePack.js'
  gsap.registerPlugin(SlowMo)
  
  onMount(() => {
    gsap.fromTo(
      '#element', 
      { x: '-20vw', rotate: gsap.utils.random(-50, -25), force3D: true },
      { x: '120vw', rotate: gsap.utils.random(25, 50), ease: 'slow(0.95, 0.5, false)', force3D: true, duration: 5 })
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
    left: 0;
    transform: translate(-50%, -50%);
    background-color: #00bb00;
  }
</style>