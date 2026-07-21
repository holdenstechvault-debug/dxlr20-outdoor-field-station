# Start Here

This ZIP contains every **project file** needed for the DX-LR20 Raspberry Pi
Control Center:

- Raspberry Pi controller and `systemd` service
- Raspberry Pi installers and uninstallers
- CSI camera test
- USB Wi-Fi hotspot support
- Web dashboard installer
- Windows graphical control application
- Windows command-line control application
- Heltec WiFi LoRa 32 V3 Arduino sketch
- Complete GitHub-style documentation
- MkDocs configuration
- GitHub issue templates
- Checksums and release manifest

External software such as Raspberry Pi OS, Raspberry Pi Imager, Arduino IDE,
Python, and the Heltec Arduino board package is not redistributed in this ZIP.
The guide gives the exact installation steps for those dependencies.

## Recommended installation order

1. Read [`README.md`](README.md).
2. Flash Raspberry Pi OS using
   [`docs/setup/os.md`](docs/setup/os.md).
3. Configure hardware using
   [`docs/setup/hardware.md`](docs/setup/hardware.md).
4. Configure all radios using
   [`docs/setup/radio.md`](docs/setup/radio.md).
5. Copy this repository to the Pi and run:

   ```bash
   cd ~/DXLR20-Control-Center-Complete-Release/software/pi
   chmod +x *.sh *.py
   sudo bash install_complete_project.sh
   ```

6. Upload the Heltec sketch from:

   ```text
   software/heltec/Heltec_V3_Pi3B_Control_Remote_v3_3_Battery.ino
   ```

7. On Windows, run:

   ```text
   software\pc-gui\run_control_center.bat
   ```

8. Follow [`docs/setup/first-test.md`](docs/setup/first-test.md).

## Uploading to GitHub

See [`UPLOAD_TO_GITHUB.md`](UPLOAD_TO_GITHUB.md). After uploading, the
repository URL can be used as the main project link.
