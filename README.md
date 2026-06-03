# My First PCB - LED Flashlight & Tester

A simple, custom-designed hardware circuit that lights up an LED when a tactile push-button is pressed. This project was created to master the fundamentals of schematic capture, footprint assignment, PCB routing, and 3D visualization in KiCad.

---

## Visuals

| Front Design (3D Render) | Back Design (With Custom Text) |
| :---: | :---: |
| ![Front View](My%20First%20Pcb/3D-View.png) | ![Back View](path/to/your/back_screenshot.png) |


---

## How It Works

The circuit is designed as a continuous power loop utilizing standard hobby components:
1. **Power Source:** A 3V CR2032 coin cell battery.
2. **Control:** A standard 4-pin 6mm tactile push-button switch that bridges the circuit when pressed.
3. **Protection:** A 220Ω current-limiting resistor to protect the LED from burning out.
4. **Output:** A 5mm red LED that lights up when the loop is securely closed.

### Circuit Loop Architecture
`Battery (+) ──> Switch ──> 220Ω Resistor ──> LED (Anode to Cathode) ──> Battery (-)`

---

## PCB Design Specifications

* **Software Used:** KiCad v8 
* **Layers:** 2-Layer Board
* **Trace Width:** 0.50 mm (Thicker traces for secure power distribution and easier hand-soldering)
* **Board Edges:** Custom rectangular `Edge.Cuts` profile with integrated hardware spacing.
* **Custom Backside:** Features custom-sized, mirrored text printed in crisp white ink on the `B.Silkscreen` layer.

---

## Bill of Materials (BOM)

| Reference | Component | Quantity | Description / Footprint |
| :--- | :--- | :---: | :--- |
| **BT1** | CR2032 Battery | 1 | Through-hole coin cell holder (Keystone 3002) |
| **SW1** | SW_Push | 1 | 6mm Tactile Push Button (SW_PUSH_6mm) |
| **R1** | Resistor | 1 | 220Ω Axial Resistor (Horizontal DIN0207) |
| **D1** | LED | 1 | 5mm Round THT LED (LED_D5.0mm) |

---

