<script>
  import { Canvas } from '@threlte/core';
  import SceneOne from '$lib/SceneOne.svelte'
  import SceneTwo from '$lib/SceneTwo.svelte'
</script>

<section>
  <h2> Scene one </h2>
  <div class="canvas-wrapper">
    <Canvas>
      <SceneOne /> 
    </Canvas>
  </div>
</section>

<section>
  <h2> Scene Two </h2>
  <div class="canvas-wrapper">
    <Canvas>
      <SceneTwo /> 
    </Canvas>
  </div>
</section>

  <style>
  .canvas-wrapper{
    position:relative;
    border:1px solid black;
    height: 500px;
  }
  </style>
