canvas-gauge
============

# Canvas Gauge v0.1

An HTML5 Canvas gauge with glow and animation.

http://www.fabledweb.com/html5-canvas-gauge.html

## Usage

```javascript
//get the canvas element that you want the gauge drawn on
var my_canvas_obj= document.getElementById("my-canvas-element");

//create a configured gauge
var gauge= new fabledweb.Gauge({
        "tick_length": 80,
        "large_tick_length": 110,
        "tick_thickness": 6,
        "num_sub_ticks": 8,
        "total_degrees": 140,
        "tick_color": "#555962",
        "tick_on_color": "#527d98",
        "tick_on_glow": 35,
        "bg_image": null,
        "gauge_scale": 0.9,
        "animation_duration": 550,
        "percent": 70,
        "canvas": my_canvas_object
});

gauge.render(); //render the configured gauge

gauge.updatePercent(30); //animate the gauge to 30%
```

To see the gauge in action and to use a UI to create a configured
gauge of your own, visit [fabledweb.com/html5-canvas-gauge.html](http://www.fabledweb.com/html5-canvas-gauge.html)

### Compatibility for that one annoying browser

Don't forget to use [explorercanvas](http://code.google.com/p/explorercanvas/)
so that this will work in browsers that don't support the HTML5 Canvas (I'm looking at you IE).
