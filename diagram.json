{
  "version": 1,
  "author": "Uri Shaked",
  "editor": "wokwi",
  "parts": [
    { "type": "wokwi-arduino-uno", "id": "uno", "top": 183, "left": 18.6, "attrs": {} },
    {
      "type": "wokwi-buzzer",
      "id": "buzzer",
      "top": 16,
      "left": 124,
      "attrs": { "volume": "0.1" }
    },
    { "type": "wokwi-led", "id": "led-red", "top": 10, "left": 6, "attrs": { "color": "red" } },
    {
      "type": "wokwi-led",
      "id": "led-green",
      "top": 73,
      "left": 6,
      "attrs": { "color": "green" }
    },
    {
      "type": "wokwi-led",
      "id": "led-blue",
      "top": 10,
      "left": 270,
      "attrs": { "color": "blue" }
    },
    {
      "type": "wokwi-led",
      "id": "led-yellow",
      "top": 73,
      "left": 270,
      "attrs": { "color": "yellow" }
    },
    {
      "type": "wokwi-pushbutton",
      "id": "btn-red",
      "top": 10,
      "left": 46,
      "attrs": { "color": "red", "key": "1", "label": "1" }
    },
    {
      "type": "wokwi-pushbutton",
      "id": "btn-green",
      "top": 76,
      "left": 46,
      "attrs": { "color": "green", "key": "2", "label": "2" }
    },
    {
      "type": "wokwi-pushbutton",
      "id": "btn-blue",
      "top": 10,
      "left": 200,
      "attrs": { "color": "blue", "key": "3", "label": "3" }
    },
    {
      "type": "wokwi-pushbutton",
      "id": "btn-yellow",
      "top": 76,
      "left": 200,
      "attrs": { "color": "yellow", "key": "4", "label": "4" }
    },
    {
      "type": "wokwi-74hc595",
      "id": "sr1",
      "top": 171.8,
      "left": 361.16,
      "rotate": 180,
      "attrs": {}
    },
    {
      "type": "wokwi-74hc595",
      "id": "sr2",
      "top": 171.8,
      "left": 457.16,
      "rotate": 180,
      "attrs": {}
    },
    { "type": "wokwi-7segment", "id": "sevseg1", "top": 47.16, "left": 379.48, "attrs": {} },
    { "type": "wokwi-7segment", "id": "sevseg2", "top": 47.16, "left": 446.68, "attrs": {} }
  ],
  "connections": [
    [ "uno:GND.1", "buzzer:1", "black", [ "v-12", "*", "h0" ] ],
    [ "uno:2", "btn-yellow:1.l", "gold", [ "v-48", "*", "h-6" ] ],
    [ "uno:GND.1", "btn-yellow:2.r", "black", [ "v-12", "*", "h6" ] ],
    [ "uno:3", "btn-blue:1.l", "blue", [ "v-44", "*", "h-10" ] ],
    [ "uno:GND.1", "btn-blue:2.r", "black", [ "v-12", "*", "h6" ] ],
    [ "uno:4", "btn-green:2.r", "green", [ "v-40", "*", "h6" ] ],
    [ "uno:GND.1", "btn-green:1.l", "black", [ "v-12", "*", "h-6" ] ],
    [ "uno:5", "btn-red:2.r", "orange", [ "v-36", "*", "h10" ] ],
    [ "uno:GND.1", "btn-red:1.l", "black", [ "v-12", "*", "h-6" ] ],
    [ "uno:8", "buzzer:2", "purple", [ "v-32", "*", "h0" ] ],
    [ "uno:9", "led-yellow:A", "gold", [ "v-28", "*", "h0" ] ],
    [ "uno:GND.1", "led-yellow:C", "black", [ "v-12", "*", "h-15", "v4" ] ],
    [ "uno:10", "led-blue:A", "blue", [ "v-24", "*", "h8" ] ],
    [ "uno:GND.1", "led-blue:C", "black", [ "v-12", "*", "h-15", "v4" ] ],
    [ "uno:11", "led-green:A", "green", [ "v-20", "*", "h0" ] ],
    [ "uno:GND.1", "led-green:C", "black", [ "v-12", "*", "h-8", "v4" ] ],
    [ "uno:12", "led-red:A", "orange", [ "v-16", "*", "h6" ] ],
    [ "uno:GND.1", "led-red:C", "black", [ "v-12", "*", "h-8", "v4" ] ],
    [ "uno:5V", "sr1:VCC", "red", [ "v57.5", "h253.4" ] ],
    [ "uno:A2", "sr1:SHCP", "gray", [ "v19.1", "h138.4" ] ],
    [ "uno:A1", "sr1:STCP", "purple", [ "v28.7", "h157.5" ] ],
    [ "uno:A0", "sr1:DS", "blue", [ "v38.3", "h186.2" ] ],
    [ "sr1:SHCP", "sr2:SHCP", "gray", [ "v47", "h106.12" ] ],
    [ "sr1:STCP", "sr2:STCP", "purple", [ "v37.4", "h96.52" ] ],
    [ "sr1:Q7S", "sr2:DS", "blue", [ "h0.52", "v56.6", "h144" ] ],
    [ "sr1:VCC", "sr1:MR", "red", [ "v17", "h-57.6" ] ],
    [ "sr1:VCC", "sr2:MR", "red", [ "v17", "h38.4" ] ],
    [ "sr1:VCC", "sr2:VCC", "red", [ "v17", "h96" ] ],
    [ "sr1:OE", "sr2:OE", "black", [ "v26.6", "h96" ] ],
    [ "sr1:MR", "sevseg1:COM.1", "red", [ "v17", "h-57.6", "v-96", "h76.8" ] ],
    [ "sevseg1:COM.1", "sevseg2:COM.1", "red", [ "h0", "v9.6", "h57.6" ] ],
    [ "sr2:Q0", "sevseg2:A", "green", [ "v7.4", "h28.8", "v-182.4", "h-67.2" ] ],
    [ "sr2:Q1", "sevseg2:B", "green", [ "v0", "h9.6", "v-134.4", "h-48" ] ],
    [ "sr2:Q2", "sevseg2:C", "green", [ "v-38.4", "h-38.4" ] ],
    [ "sr2:Q3", "sevseg2:D", "green", [ "v-33.6", "h-33.6", "v-9.6", "h-14.4" ] ],
    [ "sr2:Q4", "sevseg2:E", "green", [ "v-28.8", "h-28.8", "v-9.6", "h-14.4" ] ],
    [ "sr2:Q5", "sevseg2:F", "green", [ "v-24", "h-24", "v-9.6", "h-24", "v-110.4", "h19.2" ] ],
    [ "sr2:Q6", "sevseg2:G", "green", [ "v-19.2", "h-43.2", "v-115.2", "h14.4" ] ],
    [ "sr1:GND", "sr2:GND", "black", [ "v-9.6", "h96" ] ],
    [ "sr1:Q1", "sevseg1:B", "green", [ "v-134.4", "h-19.2" ] ],
    [ "sr1:Q2", "sevseg1:C", "green", [ "v-38.4", "h-19.2" ] ],
    [ "sr1:Q3", "sevseg1:D", "green", [ "v-33.6", "h-24" ] ],
    [ "sr1:Q4", "sevseg1:E", "green", [ "v-28.8", "h-28.8" ] ],
    [ "uno:GND.3", "sr1:GND", "black", [ "v47.9", "h157.6", "v-259.2", "h9.6" ] ],
    [ "sr1:GND", "sr1:OE", "black", [ "v-9.6", "h-9.6", "v67.2", "h172.8" ] ],
    [ "sr1:Q0", "sevseg1:A", "green", [ "v65", "h-76.8", "v-240", "h57.6" ] ],
    [ "sr1:Q5", "sevseg1:F", "green", [ "v-24", "h-19.2", "v-110.4", "h19.2" ] ],
    [ "sr1:Q6", "sevseg1:G", "green", [ "v-19.2", "h-14.4", "v-110.4", "h14.4" ] ]
  ]
}