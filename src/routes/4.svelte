<script>
  import { onMount } from 'svelte'
  import { gsap } from 'gsap'

  let element
  
  onMount(() => {
    gsap.fromTo(
      element, 
      { left: gsap.utils.random(window.innerWidth / 10, window.innerWidth / 10 * 9), rotate: gsap.utils.random(-20, 20), force3D: true },
      { top: '25%', rotate: gsap.utils.random(-20, 20), ease: 'expo', force3D: true, duration: 2, onComplete: () => { 
          gsap.to(
            element, 
            { top: "120vh", rotate: gsap.utils.random(-20, 20), ease: 'expo.in', duration: 2 })}
      })
  })
</script>


<div bind:this={element} id='element'></div>


<style>
  :global(body) {
    overflow: hidden;
  }
  
  #element {
    display: block;
    height: 150px;
    width: 150px;
    margin: 1rem;
    padding: 0;

    position: absolute;
    top: calc(100% + 150px / 2);
    left: 0;
    transform: translate(-50%, -50%);
    background-color: #00bb00;
  }
</style>