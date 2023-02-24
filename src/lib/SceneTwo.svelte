<script>
  import {PerspectiveCamera,DirectionalLight,AmbientLight} from "@threlte/core";
  import { GLTF } from "@threlte/extras";

  let url = "Duck.gltf";

</script>

  <PerspectiveCamera
  position= {{y:5,z:10}}
  lookAt= {{y:0}}
  />

<DirectionalLight/>
<AmbientLight/>

<GLTF url={url} />

