# TicTacAlc
What does it do: <br>
You can play TicTacToe with your bulbs in HomeAssistant.

<br>

What it looks like:<br>
In HomeAssistant: <br>

<img src="/doc/vid/Homeassistant.gif" width="400">

<br>

With the Bulbs:<br>

<img src="/doc/vid/Demo.gif" width="400">

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
- light.arduino_section_1
- light.arduino_section_2
- light.arduino_section_3
- light.arduino_section_4
- light.arduino_section_5
- light.arduino_section_6
- light.arduino_section_7
- light.arduino_section_8
- light.arduino_section_9

<br>
<br>

## NodeRed
Use my NodeRed code from here: [Code](/doc/code/NodeRed)

If you use my helpers and my light entitys, it should recocnize all of them. <br>
If you want to use your own ones instead, you have to change the nodes in the picture below: <br>

<img src="/doc/pic/NodeRed.png" width="500">
<br>
<br>

## Localization
Most strings are defined in Homeassistant, you have to edit them there. <br>
For P1 wins, P2 wins draw and clear you have to edit a Node in NodeRed

<br>
Edit the "winner" node: <br>

<img src="/doc/pic/String_1.png" width="500">

<br>

Edit the strings in the pic: <br>

<img src="/doc/pic/String_2.png" width="500">

<br>
<br>

## Extra
If you use the ESPHome Integration, you can setup some cool stuff too on it. <br>
Use my ESPHome code from here: [Code](/doc/code/ESPHome) <br>
With this code you get some effects for your arduino board like wled, e131 (ledfx) and some effects (rainbow, color wipe, fireworks, etc.)

<br>
<br>


## Credits
To [zenofmud](https://discourse.nodered.org/u/zenofmud/summary) for his [Tic-Tac-Toe Code](https://discourse.nodered.org/t/tic-tac-toe-game/23831) where this project is based off.
