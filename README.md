An attempt to combine the Arduino Nano modules with SMD components.

The PCB is a 10x10cm board, that is divided into 2 5x10cm fields.

On the front side the are footprints for:
* upper field:
  * LM7805 and LM1117 for 5V and 3,3V power supply (with capacitors and inductance)
  * MCP1501 voltage refference
  * voltage divider with BAV99 protection diodes
  * generic dual opamp with input and feedback resistors
  * SOT-23 transistor with biasing resistors (select which resistors to populate and which to short-out/leave out in order to obtain the desired circuuit - see examples sheet for very simple examples)
  * 6x1208/0805 (the footprint should fit both 1206 and 0805 sizes)
  * half of the pins of the Arduino module
  * pads for GND, 5V, 3,3V
* lower field:
  *  1xSOIC-28 footprint
  *  1xSOIC-8
  *  4xSOT-23
  *  11x1208/0805 (the footprint should fit both 1206 and 0805 sizes)
  *  dual output power output with DMP4025 and 2N7002. !!! GND is not provided on board, has to be provided via wire !!!
  *  pads for GND, 5V, 3,3V
![front side](/docs/smd-testboard-front.png)

On the back side the are footprints for:
* upper field:
  * generic dual opamp with input and feedback resistors
  * 3xSOT-23 transistor with biasing resistors (select which resistors to populate and which to short-out/leave out in order to obtain the desired circuuit - see examples sheet for very simple examples)
  * 8x1208/0805 (the footprint should fit both 1206 and 0805 sizes)
  * half of the pins of the Arduino module
  * pads for GND, 5V, 3,3V
* lower field:
  *  1xSOIC-28 footprint
  *  1xSOIC-8
  *  4xSOT-23
  *  10x1208/0805 (the footprint should fit both 1206 and 0805 sizes)
  *  pads for GND, 5V, 3,3V
![back side](/docs/smd-testboard-back.png)
