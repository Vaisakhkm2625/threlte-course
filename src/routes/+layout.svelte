<script>
  import { Canvas } from '@threlte/core';
  import SceneOne from '$lib/SceneOne.svelte'
</script>

<section>
  <h2> Scene one </h2>
  <div class="canvas-wrapper">
    <Canvas>
      <!--<SceneOne /> -->
      <SceneOne /> 

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
