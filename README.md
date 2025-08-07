# MLX90640ThermalCamera
MLX90640 Thermal Camera with Raspberry Pi Pico and Python Heatmap Viewer
Hardware Required
Raspberry Pi Pico or Pico W
MLX90640 thermal camera (I2C)
Micro USB cable
Jumper wires

Wiring (Pico GPIO)
SDA (data): GPIO 0
SCL (clock): GPIO 1
VCC: 3.3V
GND: GND

Arduino Sketch (Upload to Pico)
using the Earle Philhower Pico core in Arduino.( https://github.com/earlephilhower/arduino-pico/releases/download/global/package_rp2040_index.json)
Required Libraries:
Adafruit MLX90640
Adafruit BusIO

Running the System
Upload the Arduino sketch to the Pico
Plug in the Pico via USB (don’t open Serial Monitor)
Run the Python script:
python heatmap_viewer.py
A heatmap window will display live MLX90640 data!

Troubleshooting
PermissionError on COM port → Close Arduino Serial Monitor
Wrong COM port → Update SERIAL_PORT in Python
No data showing → Check wiring, sensor power, and that Pico sketch is running
