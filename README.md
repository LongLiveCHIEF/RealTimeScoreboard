# Real Time Scoreboard

A Christmas Present

**Bill Of Materials**

| Part | Quantity | Notes |
| ---- | -------- | ----- |
| 5m WS2813 60 LED/m Strip | 5 | WS2813 preferred so one pixel doesn't take out a whole line |
| ESP-32s | 1 | Microcontroller |
| Particle Boron | 1 | Microcontroller |
| 74AHCT125 | 1 | Level Shifter IC |
| 74HC595 | 4 | Shift Register IC | 
| Diffuser screen | 1 | 709.6125 mm X  403.225 mm |
|[DC 5V 60A 300W Regulated Transformer Power Supply](https://www.amazon.com/gp/product/B07C6NSRJC/ref=ppx_yo_dt_b_asin_title_o00_s00?ie=UTF8&psc=1) | 1 | Scavenged from 32 LED Flatscreen TV |

 **Array Size/Power Details:**
 - W x H = 42 x 33
 - Each 1 pixel segment = W x H = 16.5 mm x 10 mm
 - Each row has 2 mm  margin on top 
 - Each Pixel can consume 0.3W at peak power
 - 1386 pixels x 0.3W = 415W at peak current
 - 415 Watts / 5 Volts = 83 Amps
 - realistic usage should be half of that, so to be safe power supply will be
 5V 60A 300W
