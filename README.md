# thinkfan.yaml
#ThinkPad T490:
sensors:
#thinkpad-isa-0000/ISA adapter
- hwmon: /sys/devices/platform/thinkpad_hwmon/hwmon
indices: [1, 2, 3, 4, 5, 6, 7, 9, 10, 11, 12, 13, 14, 15, 16]
correction: [0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0]
- hwmon: /sys/devices/platform/coretemp.0/hwmon/
indices: [1, 2, 3, 4, 5]
correction: [0, 0, 0, 0, 0]
optional: true
- hwmon: /sys/devices/pci0000:00/0000:00:1d.4/0000:3d:00.0/hwmon/
indices: [1, 2, 3]
correction: [0, 0, 0]
- hwmon: /sys/devices/virtual/thermal/thermal_zone6/
indices: [1]
correction: [0]
- hwmon: /sys/devices/virtual/thermal/thermal_zone0/hwmon0/
indices: [1]
correction: [0]
- hwmon: /sys/devices/virtual/thermal/thermal_zone4/
indices: [1]
correction: [0]
fans:
- tpacpi: /proc/acpi/ibm/fan
levels:
- [0, 0, 50]
- [1, 50, 52]
- [2, 52, 54]
- [4, 55, 62]
- [5, 60, 67]
- [6, 65, 72]
- ["level auto", 54, 75]
- ["level disengaged", 70, 255]
