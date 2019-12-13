# Real Time Scoreboard

A Christmas Present for my brother. 

## Overview

My brother is a huge Chicago Bulls and St Louis Cardinals fan. He has a room dedicated to
these two teams. He also spends a lot of time driving around the city, and me being an
electronics maker, ask him to keep an eye out for discarded electronics.

One day he picked up a 32 flatscreen LED tv that had no power cord, and asked if I could get
it working. It wasn't meant to be... however when I took it apart for parts, I had an idea.

I thought my brothers sports room would be that much more immersive if there was a 32" "pixelized"
real-time scoreboard whenever one of his favorite teams play.

When the Bulls are playing, I imagine it would look like a common basketball scoreboard you might
see in a high school gym, complete with a shot clock (if possible)

When the Cards are playing, I want the display to look like the outfield scoreboard with box scores.

When games aren't playing, I want to have a few screens with just the respective team logos displaying,
and see if I can maybe list each teams hall of fame stats or something.

That's the plan as of now, at the start of this project. Watch the project to see my progress.

I'll be open sourcing all code, 3D designs, and circuit schematics for this project so you can make your
own if I'm successful, or improve on my failures if I'm not!

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
