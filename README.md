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
```

```
```

```
```



