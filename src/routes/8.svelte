<script>
  import { onMount } from 'svelte'
  import { gsap } from 'gsap'
  import { ScrollToPlugin } from 'gsap/dist/ScrollToPlugin';
  gsap.registerPlugin(ScrollToPlugin);

  let anchor
  
  onMount(() => {
    anchor.onclick = (event) => {
      event.preventDefault()
      gsap.to(
        window, 
        { scrollTo: event.target.getAttribute('href'), ease: 'expo.inOut' }
      )
    }
  })
</script>


<p><a href='#index' bind:this={anchor}>Scroll to Index</a></p>

<p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Quisque id diam vel quam. Ipsum suspendisse ultrices gravida dictum. Id volutpat lacus laoreet non curabitur gravida. Pellentesque adipiscing commodo elit at imperdiet dui accumsan. Urna molestie at elementum eu facilisis sed odio morbi quis. Hendrerit dolor magna eget est lorem ipsum. Nunc sed id semper risus in hendrerit gravida rutrum. Consectetur a erat nam at lectus urna. Massa vitae tortor condimentum lacinia quis vel eros donec ac. Tortor pretium viverra suspendisse potenti nullam ac tortor vitae purus. Leo urna molestie at elementum eu facilisis sed odio morbi. Condimentum lacinia quis vel eros donec.</p>

<p>Nunc eget lorem dolor sed viverra ipsum nunc aliquet bibendum. Nibh sit amet commodo nulla facilisi nullam vehicula ipsum a. Sapien pellentesque habitant morbi tristique senectus. Libero enim sed faucibus turpis in. Magna fermentum iaculis eu non diam phasellus vestibulum lorem. Interdum velit laoreet id donec ultrices tincidunt arcu non sodales. Id donec ultrices tincidunt arcu non sodales neque sodales ut. Ut etiam sit amet nisl purus in mollis. Cras sed felis eget velit aliquet sagittis id. Tortor vitae purus faucibus ornare suspendisse sed nisi lacus. Felis bibendum ut tristique et egestas quis ipsum suspendisse. Sit amet nisl suscipit adipiscing bibendum. Enim ut tellus elementum sagittis vitae et. Tortor at auctor urna nunc id cursus metus. Magna sit amet purus gravida quis blandit. Tellus at urna condimentum mattis pellentesque id nibh tortor id.</p>

<p>At in tellus integer feugiat scelerisque varius. Viverra suspendisse potenti nullam ac. Semper risus in hendrerit gravida rutrum quisque non tellus. Duis ultricies lacus sed turpis. Justo laoreet sit amet cursus sit. Pharetra et ultrices neque ornare. Lectus sit amet est placerat in egestas erat. In ornare quam viverra orci sagittis eu volutpat odio. Sed cras ornare arcu dui vivamus arcu felis. Sagittis vitae et leo duis. Bibendum arcu vitae elementum curabitur vitae nunc sed. Elementum eu facilisis sed odio morbi quis commodo odio. Lacus vel facilisis volutpat est velit egestas dui. Vel facilisis volutpat est velit. Ut eu sem integer vitae justo. Mi quis hendrerit dolor magna eget est lorem ipsum. Morbi tincidunt augue interdum velit euismod in. Orci a scelerisque purus semper eget duis at tellus at.</p>

<p>Elementum nisi quis eleifend quam adipiscing vitae. Volutpat lacus laoreet non curabitur gravida arcu ac. Imperdiet massa tincidunt nunc pulvinar sapien et ligula ullamcorper malesuada. Aliquam id diam maecenas ultricies mi eget mauris. Risus quis varius quam quisque. Sem nulla pharetra diam sit amet. Elementum facilisis leo vel fringilla est ullamcorper. Tortor condimentum lacinia quis vel eros donec ac odio tempor. Curabitur gravida arcu ac tortor dignissim convallis aenean et tortor. Enim ut tellus elementum sagittis vitae et leo duis ut. Velit scelerisque in dictum non consectetur a.</p>

<p>Egestas integer eget aliquet nibh praesent tristique magna sit amet. Ut lectus arcu bibendum at. Et ultrices neque ornare aenean. Eget duis at tellus at urna condimentum mattis. Mattis enim ut tellus elementum. Diam quis enim lobortis scelerisque fermentum dui faucibus. Id velit ut tortor pretium. Ante metus dictum at tempor commodo ullamcorper a. Ac turpis egestas integer eget aliquet nibh praesent tristique magna. Convallis convallis tellus id interdum velit laoreet. Sit amet purus gravida quis. Ipsum consequat nisl vel pretium lectus. Vitae semper quis lectus nulla at volutpat. Etiam non quam lacus suspendisse faucibus. Elit ut aliquam purus sit amet. Eget lorem dolor sed viverra. Eget magna fermentum iaculis eu non diam. Mauris a diam maecenas sed. Sed nisi lacus sed viverra tellus in hac habitasse. Quis auctor elit sed vulputate mi sit amet mauris commodo.</p>

<p>Nisl tincidunt eget nullam non nisi est. Dui ut ornare lectus sit amet est placerat in egestas. Vitae congue mauris rhoncus aenean vel elit scelerisque. Ultricies integer quis auctor elit sed vulputate mi sit amet. Lacus sed viverra tellus in hac habitasse. Id faucibus nisl tincidunt eget. Sem viverra aliquet eget sit amet tellus cras adipiscing. Lobortis feugiat vivamus at augue eget arcu dictum. Velit aliquet sagittis id consectetur purus. Tristique risus nec feugiat in. Eu nisl nunc mi ipsum faucibus vitae aliquet nec ullamcorper. Odio pellentesque diam volutpat commodo sed. Mollis nunc sed id semper risus in hendrerit gravida rutrum. Sit amet consectetur adipiscing elit pellentesque habitant morbi tristique. Viverra ipsum nunc aliquet bibendum. Lectus nulla at volutpat diam ut venenatis tellus in.</p>

<p>At quis risus sed vulputate odio. Tempor orci dapibus ultrices in iaculis nunc sed augue. Pretium nibh ipsum consequat nisl vel pretium lectus quam. Ornare arcu odio ut sem. Eu turpis egestas pretium aenean pharetra magna ac placerat. Eleifend mi in nulla posuere sollicitudin aliquam ultrices. Consequat mauris nunc congue nisi. Suspendisse in est ante in nibh mauris cursus mattis. Ut tortor pretium viverra suspendisse potenti nullam ac tortor vitae. Phasellus faucibus scelerisque eleifend donec pretium vulputate. Tellus rutrum tellus pellentesque eu tincidunt tortor. Ac tortor dignissim convallis aenean et tortor at risus viverra. Nisl vel pretium lectus quam id leo in. Neque gravida in fermentum et sollicitudin ac.</p>

<p id='index'>Index</p>

<p>Placerat orci nulla pellentesque dignissim. In est ante in nibh mauris cursus mattis. Leo urna molestie at elementum eu facilisis sed odio. Ullamcorper dignissim cras tincidunt lobortis feugiat vivamus at. Orci phasellus egestas tellus rutrum tellus pellentesque eu tincidunt tortor. Nulla pharetra diam sit amet nisl suscipit. Ultricies tristique nulla aliquet enim tortor. Tempor orci dapibus ultrices in iaculis nunc. Eget lorem dolor sed viverra ipsum nunc aliquet bibendum enim. Euismod in pellentesque massa placerat duis ultricies lacus sed turpis. Ut enim blandit volutpat maecenas volutpat blandit aliquam etiam erat. Id ornare arcu odio ut sem. Mattis molestie a iaculis at erat pellentesque. Pharetra sit amet aliquam id diam maecenas ultricies mi eget. Et tortor consequat id porta nibh venenatis cras sed. Netus et malesuada fames ac turpis egestas. Varius vel pharetra vel turpis nunc eget. Pellentesque pulvinar pellentesque habitant morbi tristique senectus et. Sed augue lacus viverra vitae congue eu consequat ac.</p>

<p>Neque egestas congue quisque egestas. Pellentesque massa placerat duis ultricies lacus sed turpis tincidunt. Purus sit amet luctus venenatis lectus magna fringilla urna porttitor. Mi eget mauris pharetra et ultrices neque ornare aenean. Id diam vel quam elementum. Magnis dis parturient montes nascetur ridiculus mus mauris vitae ultricies. Arcu non sodales neque sodales ut etiam sit. Pellentesque massa placerat duis ultricies lacus sed turpis tincidunt. Eget nunc lobortis mattis aliquam faucibus purus in massa tempor. Auctor eu augue ut lectus arcu bibendum at. Consectetur adipiscing elit ut aliquam purus.</p>

<p>Nisl tincidunt eget nullam non nisi est. Dui ut ornare lectus sit amet est placerat in egestas. Vitae congue mauris rhoncus aenean vel elit scelerisque. Ultricies integer quis auctor elit sed vulputate mi sit amet. Lacus sed viverra tellus in hac habitasse. Id faucibus nisl tincidunt eget. Sem viverra aliquet eget sit amet tellus cras adipiscing. Lobortis feugiat vivamus at augue eget arcu dictum. Velit aliquet sagittis id consectetur purus. Tristique risus nec feugiat in. Eu nisl nunc mi ipsum faucibus vitae aliquet nec ullamcorper. Odio pellentesque diam volutpat commodo sed. Mollis nunc sed id semper risus in hendrerit gravida rutrum. Sit amet consectetur adipiscing elit pellentesque habitant morbi tristique. Viverra ipsum nunc aliquet bibendum. Lectus nulla at volutpat diam ut venenatis tellus in.</p>


<style>
  p {
    width: 700px;
    height: auto;
    margin: 1rem;
    padding: 0;

    font-family: Arial, Helvetica, sans-serif;
    font-size: 1.25rem;
  }

  a {
    text-decoration: none;
    color: inherit;
    font-size: 2rem;
  }

  #index {
    font-size: 2rem;
  }
</style>