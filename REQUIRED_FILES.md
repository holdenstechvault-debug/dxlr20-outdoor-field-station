# Required Files

## Files included in this release

### Raspberry Pi

| File | Purpose |
|---|---|
| `software/pi/dxlr20_pi3b_reliable.py` | Main LoRa command handler, CSI camera capture, system controls, and IMG2 image transmitter |
| `software/pi/dxlr20-pi3b-reliable.service` | Starts the Pi controller automatically at boot |
| `software/pi/install_or_update_pi_v3.sh` | Installs or updates the main Pi controller |
| `software/pi/install_complete_project.sh` | Installs the Pi controller, web dashboard, and hotspot dashboard access |
| `software/pi/update_usb_wifi_ap.sh` | Forces hotspot use of a physical USB Wi-Fi dongle |
| `software/pi/detect_usb_wifi.sh` | Identifies the built-in and USB wireless interfaces |
| `software/pi/test_csi_camera.sh` | Tests the Pi CSI camera connector |
| `software/pi/uninstall_pi_v3.sh` | Removes the main Pi controller |

### Windows graphical application

| File | Purpose |
|---|---|
| `software/pc-gui/dxlr20_control_center.py` | Main graphical control center and IMG2 receiver |
| `software/pc-gui/run_control_center.bat` | Installs dependencies and launches the GUI |
| `software/pc-gui/build_control_center_exe.bat` | Optional executable builder |
| `software/pc-gui/requirements_pc.txt` | Python dependencies |

### Windows command-line application

| File | Purpose |
|---|---|
| `software/pc-cli/dxlr20_control_cli.py` | Terminal control client and IMG2 receiver |
| `software/pc-cli/run_control_cli.bat` | Installs dependencies and launches the CLI |
| `software/pc-cli/requirements_cli.txt` | Python dependencies |

### Heltec remote

| File | Purpose |
|---|---|
| `software/heltec/Heltec_V3_Pi3B_Control_Remote_v3_3_Battery.ino` | Grouped OLED command menu, replies, progress, and estimated internal battery percentage |

### Web dashboard

| File | Purpose |
|---|---|
| `software/dashboard/install_rpi_speed_dashboard.sh` | Installs the local Raspberry Pi system dashboard |
| `software/dashboard/enable_dashboard_over_hotspot.sh` | Exposes port 8088 through the USB Wi-Fi hotspot |

## External software installed separately

The following are required but are not redistributed inside this repository:

- Raspberry Pi Imager
- Raspberry Pi OS Lite 64-bit
- Arduino IDE
- Heltec ESP32 Arduino board package
- DX-LR20 transparent-UART firmware/configuration utility, when required by the modules
- Windows Python, when not already installed
- Git, only when uploading or cloning through Git

The installation guides explain where each item is used and the included
scripts install normal Python and Linux package dependencies automatically.
