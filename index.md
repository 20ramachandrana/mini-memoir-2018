<html> 
<head>
    <script src="https://aframe.io/releases/0.8.0/aframe.min.js"></script>
  </head>
  <body>
<a-scene>
      <a-sky color= #87CEFA></a-sky>  
<a-entity position="-.81 1.81 -67" wasd-controls>
  <a-camera>
    <a-entity cursor="fuse: true;"
          position="0 0 -3"
          geometry="primitive: ring"
          scale = ".1 .1 .1"
          material="color: black; shader: flat">
  <a-animation begin="click" easing="ease-in" attribute="scale" dur="150"
               fill="forwards" from="0.01 0.01 0.01" to=".1 .1 .1"></a-animation>
  <a-animation begin="cursor-fusing" easing="ease-in" attribute="scale" dur="1500"
               fill="backwards" from=".2 .2 .2" to="0.02 0.02 0.02"></a-animation>
</a-entity>
</a-camera>
</a-entity>
  <a-cylinder position="-3.18 -.3 -6.29" id="ground" color=#fffcc1 radius="500" height="0.1"></a-cylinder>
<a-box color="gray" scale="7 .2 2000" position="-.73 -.29 0"></a-box>
<a-entity obj-model="obj: url(https://raw.githubusercontent.com/anoncs50/Immune-System-VR/master/vr.obj); mtl: url(https://raw.githubusercontent.com/anoncs50/Immune-System-VR/master/vr.mtl)" position="0.3 0 -.8">
<a-entity obj-model="obj: url(https://raw.githubusercontent.com/anoncs50/Immune-System-VR/master/macrophage.obj); mtl: url(https://raw.githubusercontent.com/anoncs50/Immune-System-VR/master/macrophage.mtl)" position="-1.01 -.021 -.39" scale=".05 .05 .05" visible="false">
<a-animation attribute="visible" begin="6500" to="true"></a-animation>
<a-animation attribute="position" begin="7000" from="-1.01 -.021 -.39" to="-1.01 1 -.39" for="4000"></a-animation>
<a-animation attribute="position" begin="11000" from="-1.01 1 -.39" to="-1.06 1.175 -.39" for="500"></a-animation>
<a-animation attribute="position" begin="11500" from="-1.06 1.175 -.39" to="-1.06 1.671 -.39" for="2000"></a-animation>
<a-animation attribute="position" begin="13500" from="-1.06 1.671 -.39" to="-1.11 1.801 -.39" for="500"></a-animation>
<a-animation attribute="position" begin="14000" from="-1.11 1.801 -.39" to="-1.11 2.39 -.39" for="2000"></a-animation>
<a-animation attribute="visible" begin="27000" to="false"></a-animation>
</a-entity>
<!-- Pathogen 1 -->
<a-entity obj-model="obj: url(https://raw.githubusercontent.com/anoncs50/Immune-System-VR/master/pathogen.obj); mtl: url(https://raw.githubusercontent.com/anoncs50/Immune-System-VR/master/pathogen.mtl)" scale=".05 .05 .05" position="-1.89 1.889 -.45" visible="false">
<a-animation attribute="visible" begin="500" to="true"></a-animation>
<a-animation attribute="position" begin="4000" from="-1.89 1.889 -.45" to="-1.03 2.567 -.45" for="1000"></a-animation>
<a-animation attribute="visible" begin="15000" to="false"></a-animation>
</a-entity>
<!-- Pathogen 2 -->
<a-entity obj-model="obj: url(https://raw.githubusercontent.com/anoncs50/Immune-System-VR/master/pathogen.obj); mtl: url(https://raw.githubusercontent.com/anoncs50/Immune-System-VR/master/pathogen.mtl)" scale=".05 .05 .05" position="-1.89 1.889 -.45" visible="false"> 
<a-animation attribute="visible" begin="500" to="true"></a-animation>
<a-animation attribute="position" begin="4000" from="-1.89 1.889 -.45" to="-1.04 2.863 -.45" for="1000"></a-animation>
<a-animation attribute="visible" begin="40000" to="false"></a-animation>
</a-entity>
<a-entity obj-model="obj: url(https://raw.githubusercontent.com/anoncs50/Immune-System-VR/master/infresp.obj); mtl: url(https://raw.githubusercontent.com/anoncs50/Immune-System-VR/master/infresp.mtl)" position="0.114 -.02 .06">
<a-animation attribute="scale" begin="5500" from="1 1 1" to="1.1 1.1 1.1"></a-animation>
</a-entity>
<a-text value="skin with a cut" position="-1.37 1.897 -.33" color="#0000ff" rotation="0 0 -90"></a-text>
<a-text value="inflammatory response" color="#0000ff" visible="false" position="-1.76 3.541 -.53" scale=".5 .5 .5">
 <a-animation attribute="visible" begin="5500" to="true"></a-animation>   
  <a-animation attribute="visible" begin="8000" to="false"></a-animation> 
 </a-text>
<a-text value="macrophage presents antigen to the t cell" color="#0000ff" visible="false" position="-2.15 3.541 -.53" scale=".5 .5 .5">
<a-animation attribute="visible" begin="14500" to="true"></a-animation>
<a-animation attribute="visible" begin="21000" to="false"></a-animation> 
</a-text>
<a-cone color="#000000" rotation="180 0 0" scale=".04 .09 .04" position="-1.14 2.25 -.39" visible="false">
<a-animation attribute="visible" begin="16000" to="true"></a-animation>  
<a-animation attribute="visible" begin="27000" to="false"></a-animation>
</a-cone>
<a-text value="antigen" position="-1.21 2.25 -.28" color="#ffff00" scale=".25 .25 .25" visible="false">
<a-animation attribute="visible" begin="15500" to="true"></a-animation>  
<a-animation attribute="visible" begin="27000" to="false"></a-animation>    
</a-text>
<a-entity obj-model="obj: url(https://raw.githubusercontent.com/anoncs50/Immune-System-VR/master/htc.obj); mtl: url(https://raw.githubusercontent.com/anoncs50/Immune-System-VR/master/htc.mtl)" position="-1.01 -.021 -.39" scale=".07 .07 .07" visible="false">
<a-animation attribute="visible" begin="15500" to="true"></a-animation>
<a-animation attribute="position" begin="16000" from="-1.01 -.021 -.39" to="-1.01 1 -.39" for="4000"></a-animation>
<a-animation attribute="position" begin="20000" from="-1.01 1 -.39" to="-1.06 1.175 -.39" for="500"></a-animation>
<a-animation attribute="position" begin="20500" from="-1.06 1.175 -.39" to="-1.06 1.671 -.39" for="2000"></a-animation>
<a-animation attribute="position" begin="22500" from="-1.06 1.671 -.39" to="-1.11 1.801 -.39" for="500"></a-animation>
<a-animation attribute="position" begin="23000" from="-1.11 1.801 -.39" to="-1.13 1.929 -.39" for="2000"></a-animation>
<a-animation attribute="visible" begin="27000" to="false"></a-animation>
</a-entity>
<a-entity obj-model="obj: url(https://raw.githubusercontent.com/anoncs50/Immune-System-VR/master/blymph.obj); mtl: url(https://raw.githubusercontent.com/anoncs50/Immune-System-VR/master/blymph.mtl)" position="-.89 -.02 -.7" scale=".2 .2 .2" visible="false">
<a-animation attribute="visible" begin="27500" to="true"></a-animation>
<a-animation attribute="position" begin="29000" from="-.89 -.0763 -.57" to="-.89 .86 -.7" for="4000"></a-animation>
<a-animation attribute="position" begin="33000" from="-.89 .86 -.7" to="-.95 .984 -.7" for="500"></a-animation>
<a-animation attribute="position" begin="33500" from="-.95 .984 -.7" to="-.94 1.514 -.7" for="2000"></a-animation>
<a-animation attribute="position" begin="35500" from="-.95 1.514 -.7" to="-1.01 1.602 -.7" for="500"></a-animation>
<a-animation attribute="position" begin="36000" from="-1.01 1.602 -.7" to="-1 2.476 -.7" for="2000"></a-animation>
<a-animation attribute="visible" begin="40000" to="false"></a-animation>
</a-entity>
<!-- top plasma -->
<a-entity obj-model="obj: url(https://raw.githubusercontent.com/anoncs50/Immune-System-VR/master/plasmacell.obj); mtl: url(https://raw.githubusercontent.com/anoncs50/Immune-System-VR/master/plasmacell.mtl)" position="-.3 2.476 -.37" scale=".025 .025 .025" visible="false">
<a-animation attribute="visible" begin="37500" to="true"></a-animation>
<a-animation attribute="position" begin="38500" from="-1.17 2.476 -.37"  to="-1.17 2.704 -.37" for="1000"></a-animation>
<a-animation attribute="visible" begin="40000" to="false"></a-animation>
</a-entity> 
<!-- bottom plasma -->
<a-entity obj-model="obj: url(https://raw.githubusercontent.com/anoncs50/Immune-System-VR/master/plasmacell.obj); mtl: url(https://raw.githubusercontent.com/anoncs50/Immune-System-VR/master/plasmacell.mtl)" position="-.4 2.502 -.37" scale=".025 .025 .025" visible="false">
<a-animation attribute="visible" begin="37500" to="true"></a-animation>
<a-animation attribute="position" begin="38500" from="-1.17 2.502 -.37" to="-1.17 2.650 -.37" for="200"></a-animation>
<a-animation attribute="visible" begin="40000" to="false"></a-animation>
</a-entity>
<a-entity obj-model="obj: url(https://raw.githubusercontent.com/anoncs50/Immune-System-VR/master/memorycell.obj); mtl: url(https://raw.githubusercontent.com/anoncs50/Immune-System-VR/master/memorycell.mtl)" position="-1 2.476 -.7" scale=".2 .2 .2" visible="false">
<a-animation attribute="visible" begin="40000" to="true"></a-animation>
<a-animation attribute="position" begin="41000" from="-1 2.476 -.7" to="-1 1.602 -.7" for="2000"></a-animation>
<a-animation attribute="position" begin="43000" from="-1 1.602 -.7" to="-.94 1.514 -.7" for="500"></a-animation>
<a-animation attribute="position" begin="43500" from="-.94 1.514 -.7" to="-.94 .955 -.7" for="500"></a-animation>
<a-animation attribute="position" begin="44000" from="-.94 .955 -.7" to="-.89 .895 -.7" for="500"></a-animation>
<a-animation attribute="position" begin="44500" from="-.89 .895 -.7" to="-.89 -.18 -.7" for="500"></a-animation>
<a-animation attribute="visible" begin="45000" to="false"></a-animation>
</a-entity>
<a-text value="b cell notified, goes to site of pathogen" color="#0000ff" visible="false" position="-2.15 3.541 -.53" scale=".5 .5 .5">
<a-animation attribute="visible" begin="28000" to="true"></a-animation>
<a-animation attribute="visible" begin="31000" to="false"></a-animation> 
</a-text>
<a-text value="b cell replicates itself and creates plasma cells to kill the pathogen" color="#0000ff" visible="false" position="-2.15 3.541 -.53" scale=".5 .5 .5">
<a-animation attribute="visible" begin="38000" to="true"></a-animation>
<a-animation attribute="visible" begin="40000" to="false"></a-animation> 
</a-text>
<a-text value="pathogen killed, memory cells stay in bloodstream, to remove pathogen quickly when exposed to it again" color="#0000ff" visible="false" position="-2.15 3.541 -.53" scale=".5 .5 .5">
<a-animation attribute="visible" begin="42000" to="true"></a-animation>
<a-animation attribute="visible" begin="52000" to="false"></a-animation> 
</a-text>
</a-entity>
</a-scene>
  </body>
</html>
