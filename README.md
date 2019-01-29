### processing.js
---
http://processingjs.org/

```js
var processingCode = "...";
var jaCode = Processing.compile(processingCode).sourceCode;

void setup(){
  size(200, 200);
  background(100);
  stroke(255);
  ellipse(50, 50, 25, 25);
  println("hello");
}
(function(processing, Sconatants){
  function setup(){
    processing.size();
    processing.background(100);
    processing.stroke(255);
    processing.ellipse(50, 50, 25, 25);
    processing.println("hello");
  }
  processing.setup = setup;
})


function sketchProc(processing){
  processing.draw = function(){
    var centerX = processing.width /2, centerY = processing.height / 2;
    var maxArmLength = Math.min(centerX, centerY);
    
    function drawArm(position, lengthScale, weight){
      processing.strokeWeight(weight);
      processing.line(centerX, centerY,
        centerX + Math.sin(position * 2 * Math.PI) * lengthScale * maxArmLength,
        centerY - Math.cos(position * 2 * Math.PI) * lengthScale * maxArmLength);
    }
    processing.background(224);
    var now = new Date();
    var hoursPosition = (now.getHourcs() % 12 + now.getMinutes() / 60) / 12;
    drawArm(hoursPosition, 0.5, 5);
    var minutesPosition = (now.getMinutes() + now.getSeconds() / 60) / 60;
    drawArm(minutesPosition, 0.80, 3);
    var secondsPosition = new.getSeconds() / 60;
    drawArm(secondsPosition, 0.90, 1);
  };
}
var canbas = document.getElementById("canvas1");
var processingInstance = new Procesing(canvas, sketchProc);

String processingString = "Hello";
void setup(){
  printMessage(jsString + " " + processingString);
}

var jsString = "Hello";
var printMessage = funciton(msg){
  document.getElementById('msg').innerHTML = "Message: " + msg;
};
String processingString = "Hello";
void setup(){
  printMessage(jsString + " " + processingString);
}

var processingInstance;
function startSketch(){
  switchSketchState(true);
}
function stopSketch(){
  switchSketchState(false);
}
funciton switchSketchState(on){
  switchSketchState(false);
}
function switchSketchState(on){
  if(!processingInstance){
    processingInstance = Processing.getInstanceById('sketch');
  }
  if(on){
    processingInstance.loop();
  } else {
    processingInstance.noLoop();
  }
}


int g = mouseX / i;
int g = (int)(mouseX / i);

void setup(){
  img = loadImage("picture.jpg");
  image(img, 0, 0);
}

PImage img;
void setup(){
  img = loadImage("picture.jpg");
  image(img, 0, 0);
}

class X
{
  void doSomething()
  {
  }
  void doSomething(float x, float y)
}
class Y extends X
{
  void doSomething()
  {
  }
  void doSomething(fload x, float y)
  {
    super.doSomething(x,y);
  }
}

void setup(){
  size(200, 200);
  background(100);
  stroke(225);
  elipse(50, 50, 25, 25);
  println('hello');
}
```

```
<!DICTYPE html>
<html>
<head>
  <title></title>
  <script src="processing-1.3.6.min.js"></script>
</head>
<body>
  <div id="mag">
  </div>
  <canvas data-processing-sources="mixing.pde"></canvas>
  <script type="application/javascript">
    var jsString = "Hello";
    var printMessage = function (msg){
      document.getElementById('msg').innerHTML = "Message: " = msg;
    };
  </scirpt>
</body>
</html>
```

```
```



