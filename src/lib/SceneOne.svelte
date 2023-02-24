<script>
  import {
    PerspectiveCamera,
    DirectionalLight,
    AmbientLight,
    Mesh,
    useFrame
  } from "@threlte/core";

import {
 MeshStandardMaterial,IcosahedronGeometry
} from 'three'

  import { tweened } from "svelte/motion";
  const t = tweened(3, {duration:2000});

  let r=0;
  // to change on every frame
  useFrame(()=>{
    r+=0.05
  })

  /* hooks that we get from threlte relay on the context of the frame
which means it should be used inside Canvas element
  */

</script>

<PerspectiveCamera 
  position={{ y:5,z:10 }} 
  lookAt={{y:0}} >
</PerspectiveCamera>

  <DirectionalLight />
  <AmbientLight/>

<Mesh
  geometry = { new IcosahedronGeometry()}
  material = { new MeshStandardMaterial({color: 'seagreen'})}
  position= {{ x: $t }} interactive 
  rotation={{y:r}}
  on:click= {()=> $t = $t>0 ? -3:3}
  />
