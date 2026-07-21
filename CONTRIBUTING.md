# Contributing

Read [the contribution guide](docs/development/contributing.md) before modifying protocol, command, or remotely privileged behavior.

Run syntax checks before submitting changes:

```bash
python3 -m py_compile software/pi/dxlr20_pi3b_reliable.py
python3 -m py_compile software/pc-gui/dxlr20_control_center.py
python3 -m py_compile software/pc-cli/dxlr20_control_cli.py
```
