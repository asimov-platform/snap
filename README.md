# Snap Package for ASIMOV Platform

This repository provides the Snap package for the [ASIMOV Platform]

## **Prerequisites**

- A Linux distribution with [Snap support](https://snapcraft.io/docs/installing-snapd).
- Snapd installed and enabled.
- `wget` (for downloading the `.snap` file).

## **Download**

The Snap package will be downloaded into the `asimov` directory inside the home folder (`~/asimov`).

```bash
mkdir -p ~/asimov && cd ~/asimov
wget https://github.com/asimov-platform/snap/releases/download/v25.0.0-dev.3/asimov-cli_25.0.0-dev.3_amd64.snap -O asimov-cli.snap
```

## Installation

Once the download is complete, install the Snap package using:

```bash
sudo snap install --dangerous ~/asimov/asimov-cli.snap
```

## Usage

After installation, you can run the CLI with:

```bash
snap run asimov-cli.asimov --help
```

To check the installed version:

```bash
snap run asimov-cli.asimov --version
```

## Troubleshooting

If the Snap does not run as expected, check the logs:

```bash
snap logs asimov-cli
```

Ensure that Snap is installed and enabled on your system:

```bash
snap version
```

For additional help, refer to the [Snapcraft documentation](https://snapcraft.io/docs).

[ASIMOV Platform]: https://github.com/asimov-platform
[asimov-cli]: https://github.com/asimov-platform/asimov-cli
