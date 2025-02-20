# ESPHome LED Matrix Example 

![Example of a text display on an 8x8 LED matrix.](text.gif)

![A smallish analog clock on an 8x8 LED matrix.](clock.gif)

![A marquee digital clock.](marqueeclock.gif)

<a href="https://esphome.io/"><img src="https://esphome.io/_images/logo-text.png" align="left" height="48" ></a>

This is an example of how to use a LED matrix [like this](https://www.adafruit.com/product/1487) as a display for text and graphics with [ESPHome (>= v1.15)](https://esphome.io/).
It leverages the [display API of ESPhome](https://esphome.io/components/display/index.html) for [addressable lights](https://esphome.io/components/light/index.html).

The main configuration file is [matrixleddemo.yaml](matrixleddemo.yaml) wich uses a header file [my_matrixled_scrolling_display.h](my_matrixled_scrolling_display.h).
The scrolling clock and text display allows to set an arbitrary text via mqtt, for instance via:
```
	mosquitto_pub -h mqtthost... -t text/text -m "Hi there!"
```

Furthermore there is an example for the [ATOM Matrix ESP32 Development Kit](https://m5stack.com/collections/m5-atom/products/atom-matrix-esp32-development-kit) in [m5atom_marquee.yaml](m5atom_marquee.yaml).


Have fun,
[Richard](https://nauber.dev)

 

