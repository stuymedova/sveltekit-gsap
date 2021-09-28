<script>
  import { onMount } from 'svelte'
  import { gsap } from 'gsap'
  
  onMount(() => {
    const animation = () => {
      gsap.fromTo(
        '#element', 
        { scale: 0, rotate: 0 },
        { scale: 1, rotate: 180, ease: 'back(1.5)', duration: 1, onComplete: () => {
          gsap.set(document.querySelector('#element'), {
            clearProps: 'transform'
        })}
    })}

    animation()
    document.querySelector('#wrapper').onclick = () => {
      animation()
    }
  })
</script>

<div id='wrapper'>
  <div id='element'></div>
</div>

<style>
  #wrapper {
    width: 100%;
    height: 100%;
    position: absolute;
    top: 0;
    left: 0;
    cursor: pointer !important;
  }

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