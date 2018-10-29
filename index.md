<html> 
<head>
    <script src="https://aframe.io/releases/0.8.0/aframe.min.js"></script>
  </head>
  <body>
<a-scene>
      <a-sky color= #87CEFA></a-sky>  
 <a-sky color="#87CEFA"></a-sky> 
<a-entity position="-.81 1.81 73" wasd-controls>
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
<a-entity obj-model="obj: url(https://raw.githubusercontent.com/anoncs50/Immune-System-VR/master/vr.obj); mtl: url(https://raw.githubusercontent.com/anoncs50/Immune-System-VR/master/vr.mtl)" position="0.3 0 -.8"></a-entity>
<a-entity obj-model="obj: url(https://raw.githubusercontent.com/anoncs50/Immune-System-VR/master/macrophage.obj); mtl: url(https://raw.githubusercontent.com/anoncs50/Immune-System-VR/master/macrophage.mtl)" position="-.71 -.021 -1.19" scale=".05 .05 .05" visible="false">
<a-animation attribute="visible" begin="46500" to="true"></a-animation>
<a-animation attribute="position" begin="47000" from="-.71 -.021 -1.37" to="-.71 1 -1.19" for="4000"></a-animation>
<a-animation attribute="position" begin="51000" from="-.71 1 -1.19" to="-.76 1.175 -1.19" for="500"></a-animation>
<a-animation attribute="position" begin="51500" from="-.76 1.175 -1.19" to="-.76 1.671 -1.19" for="2000"></a-animation>
<a-animation attribute="position" begin="53500" from="-.76 1.671 -1.19" to="-.81 1.801 -1.19" for="500"></a-animation>
<a-animation attribute="position" begin="54000" from="-.81 1.801 -1.19" to="-.81 2.39 -1.19" for="2000"></a-animation>
<a-animation attribute="visible" begin="67000" to="false"></a-animation>
</a-entity>
<!-- Pathogen 1 -->
<a-entity obj-model="obj: url(https://raw.githubusercontent.com/anoncs50/Immune-System-VR/master/pathogen.obj); mtl: url(https://raw.githubusercontent.com/anoncs50/Immune-System-VR/master/pathogen.mtl)" scale=".05 .05 .05" position="-1.59 1.889 -1.25" visible="false">
<a-animation attribute="visible" begin="40500" to="true"></a-animation>
<a-animation attribute="position" begin="44000" from="-1.59 1.889 -1.25" to="-.73 2.567 -1.25" for="1000"></a-animation>
<a-animation attribute="visible" begin="55000" to="false"></a-animation>
</a-entity>
<!-- Pathogen 2 -->
<a-entity obj-model="obj: url(https://raw.githubusercontent.com/anoncs50/Immune-System-VR/master/pathogen.obj); mtl: url(https://raw.githubusercontent.com/anoncs50/Immune-System-VR/master/pathogen.mtl)" scale=".05 .05 .05" position="-1.59 2.07 -1.25" visible="false"> 
<a-animation attribute="visible" begin="40500" to="true"></a-animation>
<a-animation attribute="position" begin="44000" from="-1.59 1.889 -1.25" to="-.74 2.863 -1.25" for="1000"></a-animation>
<a-animation attribute="visible" begin="60000" to="false"></a-animation>
</a-entity>
<a-entity obj-model="obj: url(https://raw.githubusercontent.com/anoncs50/Immune-System-VR/master/infresp.obj); mtl: url(https://raw.githubusercontent.com/anoncs50/Immune-System-VR/master/infresp.mtl)" position="0.414 -.02 -.74">
<a-animation attribute="scale" begin="45500" from="1 1 1" to="1.1 1.1 1.1"></a-animation>
</a-entity>
<a-text value="skin with a cut" position="-1.07 1.897 -1.13" color="#0000ff" rotation="0 0 -90"></a-text>
<a-text value="inflammatory response" color="#0000ff" visible="false" position="-1.46 3.541 -1.33" scale=".5 .5 .5">
 <a-animation attribute="visible" begin="45500" to="true"></a-animation>   
  <a-animation attribute="visible" begin="48000" to="false"></a-animation> 
 </a-text>
<a-text value="macrophage presents antigen to the t cell" color="#0000ff" visible="false" position="-1.85 3.541 -1.33" scale=".5 .5 .5">
<a-animation attribute="visible" begin="54500" to="true"></a-animation>
<a-animation attribute="visible" begin="61000" to="false"></a-animation> 
</a-text>
<a-cone color="#000000" rotation="180 0 0" scale=".04 .09 .04" position="-.84 2.25 -1.19" visible="false">
<a-animation attribute="visible" begin="35500" to="true"></a-animation>  
<a-animation attribute="visible" begin="47000" to="false"></a-animation>
</a-cone>
<a-text value="antigen" position="-.91 2.25 -1.08" color="#ffff00" scale=".25 .25 .25" visible="false">
<a-animation attribute="visible" begin="35500" to="true"></a-animation>  
<a-animation attribute="visible" begin="47000" to="false"></a-animation>    
</a-text>
<a-entity obj-model="obj: url(https://raw.githubusercontent.com/anoncs50/Immune-System-VR/master/htc.obj); mtl: url(https://raw.githubusercontent.com/anoncs50/Immune-System-VR/master/htc.mtl)" position="-.71 -.021 -1.19" scale=".07 .07 .07" visible="false">
<a-animation attribute="visible" begin="35500" to="true"></a-animation>
<a-animation attribute="position" begin="36000" from="-.71 -.021 -1.37" to="-.71 1 -1.19" for="4000"></a-animation>
<a-animation attribute="position" begin="40000" from="-.71 1 -1.19" to="-.76 1.175 -1.19" for="500"></a-animation>
<a-animation attribute="position" begin="40500" from="-.76 1.175 -1.19" to="-.76 1.671 -1.19" for="2000"></a-animation>
<a-animation attribute="position" begin="42500" from="-.76 1.671 -1.19" to="-.81 1.801 -1.19" for="500"></a-animation>
<a-animation attribute="position" begin="43000" from="-.81 1.801 -1.19" to="-.83 1.929 -1.19" for="2000"></a-animation>
<a-animation attribute="visible" begin="47000" to="false"></a-animation>
</a-entity>
<a-entity obj-model="obj: url(https://raw.githubusercontent.com/anoncs50/Immune-System-VR/master/blymph.obj); mtl: url(https://raw.githubusercontent.com/anoncs50/Immune-System-VR/master/blymph.mtl)" position="-.59 -.02 -1.5" scale=".2 .2 .2" visible="false">
<a-animation attribute="visible" begin="47500" to="true"></a-animation>
<a-animation attribute="position" begin="49000" from="-.59 -.0763 -1.37" to="-.59 .86 -1.5" for="4000"></a-animation>
<a-animation attribute="position" begin="53000" from="-.59 .86 -1.5" to="-.65 .984 -1.5" for="500"></a-animation>
<a-animation attribute="position" begin="53500" from="-.65 .984 -1.5" to="-.64 1.514 -1.5" for="2000"></a-animation>
<a-animation attribute="position" begin="55500" from="-.65 1.514 -1.5" to="-.71 1.602 -1.5" for="500"></a-animation>
<a-animation attribute="position" begin="56000" from="-.71 1.602 -1.5" to="-.7 2.476 -1.5" for="2000"></a-animation>
<a-animation attribute="visible" begin="60000" to="false"></a-animation>
</a-entity>
<!-- top plasma -->
<a-entity obj-model="obj: url(https://raw.githubusercontent.com/anoncs50/Immune-System-VR/master/plasmacell.obj); mtl: url(https://raw.githubusercontent.com/anoncs50/Immune-System-VR/master/plasmacell.mtl)" position="-.7 2.476 -1.17" scale=".025 .025 .025" visible="false">
<a-animation attribute="visible" begin="57500" to="true"></a-animation>
<a-animation attribute="position" begin="58500" from="-.8 2.476 -1.17"  to="-.81 2.704 -1.17" for="1000"></a-animation>
<a-animation attribute="visible" begin="60000" to="false"></a-animation>
</a-entity> 
<!-- bottom plasma -->
<a-entity obj-model="obj: url(https://raw.githubusercontent.com/anoncs50/Immune-System-VR/master/plasmacell.obj); mtl: url(https://raw.githubusercontent.com/anoncs50/Immune-System-VR/master/plasmacell.mtl)" position="-.8 2.502 -1.17" scale=".025 .025 .025" visible="false">
<a-animation attribute="visible" begin="57500" to="true"></a-animation>
<a-animation attribute="position" begin="58500" from="-.8 2.502 -1.17" to="-.81 2.650 -1.17" for="200"></a-animation>
<a-animation attribute="visible" begin="60000" to="false"></a-animation>
</a-entity>
<a-entity obj-model="obj: url(https://raw.githubusercontent.com/anoncs50/Immune-System-VR/master/memorycell.obj); mtl: url(https://raw.githubusercontent.com/anoncs50/Immune-System-VR/master/memorycell.mtl)" position="-.7 2.476 -1.5" scale=".2 .2 .2" visible="false">
<a-animation attribute="visible" begin="60000" to="true"></a-animation>
<a-animation attribute="position" begin="61000" from="-.7 2.476 -1.5" to="-.7 1.602 -1.5" for="2000"></a-animation>
<a-animation attribute="position" begin="63000" from="-.7 1.602 -1.5" to="-.64 1.514 -1.5" for="500"></a-animation>
<a-animation attribute="position" begin="63500" from="-.64 1.514 -1.5" to="-.64 .955 -1.5" for="500"></a-animation>
<a-animation attribute="position" begin="64000" from="-.64 .955 -1.5" to="-.59 .895 -1.5" for="500"></a-animation>
<a-animation attribute="position" begin="64500" from="-.59 .895 -1.5" to="-.59 -.18 -1.5" for="500"></a-animation>
<a-animation attribute="visible" begin="65000" to="false"></a-animation>
</a-entity>
<a-text value="b cell notified, goes to site of pathogen" color="#0000ff" visible="false" position="-1.85 3.541 -1.33" scale=".5 .5 .5">
<a-animation attribute="visible" begin="48000" to="true"></a-animation>
<a-animation attribute="visible" begin="51000" to="false"></a-animation> 
</a-text>
<a-text value="b cell replicates itself and creates plasma cells to kill the pathogen" color="#0000ff" visible="false" position="-1.85 3.541 -1.33" scale=".5 .5 .5">
<a-animation attribute="visible" begin="58000" to="true"></a-animation>
<a-animation attribute="visible" begin="60000" to="false"></a-animation> 
</a-text>
<a-text value="pathogen killed, memory cells stay in bloodstream, to remove pathogen quickly when exposed to it again" color="#0000ff" visible="false" position="-1.85 3.541 -1.33" scale=".5 .5 .5">
<a-animation attribute="visible" begin="62000" to="true"></a-animation>
<a-animation attribute="visible" begin="72000" to="false"></a-animation> 
</a-text>
</a-sky> 
</a-scene>
  </body>
</html>

