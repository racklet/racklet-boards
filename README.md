# Racklet Boards

This repository documents the compatibility of different SBC boards with racklet.

## Board Dimensions

Board dimensions are collected to determine which boards are physically compatible
with the racklet form factor. SBCs mounted to the rack must have an ethernet
port available at the front panel which constrains the mounting orientation of
the SBC. In order to compare board dimensions in a consistent way we choose the
following naming convention.

Dimensions are measured wrt. the primary side, which is defined as the side
where the Ethernet port is located. If there are multiple ethernet ports,
pick the (first) one that makes the width the smallest.

![SBC front view](docs/diagrams/board-front-view.svg)

- `width` - Length of the primary side of the PCB
- `depth` - Length of the another side of the PCB.
- `height` - Height of the board measured from the bottom of the PCB to the top of the tallest component.

The width and depth represent the size of the PCB without any connectors,
while the height represents the total height from the bottom of the PCB to
the tallest point of the tallest connector (e.g. the lip on the USB connector
on the Pi 4).

The physical dimensions are collected under the file `physical.toml`.
```toml
[dimensions]
# Example dimensions for a Raspberry Pi 4 Model B
# https://datasheets.raspberrypi.com/rpi4/raspberry-pi-4-mechanical-drawing.pdf
width = 56 # millimeters
height = 18 # millimeters
depth = 85 # millimeters
```

## Contributing

Please see [CONTRIBUTING.md](CONTRIBUTING.md) and our [Code Of Conduct](CODE_OF_CONDUCT.md).

Other interesting resources include:

- [The issue tracker](https://github.com/racklet/racklet/issues)
- [The discussions forum](https://github.com/racklet/racklet/discussions)
- [The list of milestones](https://github.com/racklet/racklet/milestones)
- [The roadmap](https://github.com/orgs/racklet/projects/1)
- [The changelog](https://github.com/racklet/racklet/blob/main/CHANGELOG.md)

## Getting Help

If you have any questions about, feedback for or problems with Racklet:

- Invite yourself to the [Open Source Firmware Slack](https://slack.osfw.dev/).
- Ask a question on the [#racklet](https://osfw.slack.com/messages/racklet/) slack channel.
- Ask a question on the [discussions forum](https://github.com/racklet/racklet/discussions).
- [File an issue](https://github.com/racklet/racklet/issues/new).
- Join our [community meetings](https://hackmd.io/@racklet/Sk8jHHc7_) (see also the [meeting-notes](https://github.com/racklet/meeting-notes) repo).

Your feedback is always welcome!

## Maintainers

In alphabetical order:

- Dennis Marttinen, [@twelho](https://github.com/twelho)
- Jaakko Sirén, [@Jaakkonen](https://github.com/Jaakkonen)
- Lucas Käldström, [@luxas](https://github.com/luxas)
- Verneri Hirvonen, [@chiplet](https://github.com/chiplet)

## License

[Apache 2.0](LICENSE)
