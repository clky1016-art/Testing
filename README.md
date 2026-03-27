<!DOCTYPE html>
<html>
  <head>
    <title>Art AR Experience</title>
    <script src="https://aframe.io/releases/1.3.0/aframe.min.js"></script>
    <script src="https://raw.githack.com/AR-js-org/AR.js/master/aframe/build/aframe-ar.js"></script>
  </head>

  <body style="margin: 0px; overflow: hidden;">
    <a-scene embedded arjs="sourceType: webcam; debugUIEnabled: false;">
      
      <a-assets>
        <img id="my-layer" src="https://path-to-your-digital-art.png">
      </a-assets>

      <a-marker type="pattern" url="path/to/your/pattern-artwork.patt">
        <a-image 
          src="#my-layer" 
          position="0 0 0" 
          rotation="-90 0 0" 
          scale="1 1 1">
        </a-image>
      </a-marker>

      <a-entity camera></a-entity>
    </a-scene>
  </body>
</html>
