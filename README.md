# TicTacAlc
What does it do: <br>
You can play TicTacToe with your bulbs in HomeAssistant.

<br>

What it looks like:<br>
In HomeAssistant: <br>
![](/doc/vid/Homeassistant.gif)

<br>

With the Bulbs:<br>
VIDEO EINFÜGEN

<br>
<br>

## Stuff you need

- Working HomeAssistant installation (Supervised recommended)
- 9 Bulbs (RGB recommended)
- NodeRed (HomeAssistant integration recommended)

<br>
<br>

## Home Assistant
Use my HA code from here: [Code](/doc/code/HomeAssistant)

You have to add a few helpers for it: (or use you own ones)
- input_boolean.tictacalc_clear
- input_boolean.tictacalc_locked
- input_boolean.tictacalc_rgb_1_r
- input_boolean.tictacalc_rgb_1_g
- input_boolean.tictacalc_rgb_1_b
- input_boolean.tictacalc_rgb_2_r
- input_boolean.tictacalc_rgb_2_g
- input_boolean.tictacalc_rgb_2_b
- input_boolean.tictacalc_text

You have to adjust the variables for your bulbs, mine were:
- entity: light.arduino_section_1
- entity: light.arduino_section_2
- entity: light.arduino_section_3
- entity: light.arduino_section_4
- entity: light.arduino_section_5
- entity: light.arduino_section_6
- entity: light.arduino_section_7
- entity: light.arduino_section_8
- entity: light.arduino_section_9

<br>
<br>

## NodeRed
Use my NodeRed code from here: [Code](/doc/code/NodeRed)

If you use my helpers and my light entity's it should recocnize all of them. <br>
If you want to use your own one's instead you have to change the node's in the picture below:

![](/doc/pic/NodeRed.png)

<br>
<br>


## Extra
If you use the ESPHome Integration, you can setup some cool stuff too on it. <br>
Use my ESPHome code from here: [Code](/doc/code/ESPHome) <br>
With this code you get some effects for your arduino board like wled, e131 (ledfx) and some effects (rainbow, color wipe, fireworks, etc.)

<br>
<br>


## Credits
To [zenofmud](https://discourse.nodered.org/u/zenofmud/summary) for his [zenofmud](https://discourse.nodered.org/u/zenofmud/summary) where this project is based off.
