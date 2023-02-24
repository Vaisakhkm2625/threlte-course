<script>
  import {PerspectiveCamera,DirectionalLight,AmbientLight,OrbitControls } from "@threlte/core";
  import { GLTF } from "@threlte/extras";

  const url = "https://raw.githubusercontent.com/mrdoob/three.js/dev/examples/models/gltf/MaterialsVariantsShoe/glTF/MaterialsVariantsShoe.gltf";

</script>



  <PerspectiveCamera
  position= {{y:5,z:10}}
  lookAt= {{y:0}}
  >
  
  <OrbitControls autoRotate/>
   </PerspectiveCamera>



<DirectionalLight/>
<AmbientLight/>



<GLTF url={url} scale={30} />

