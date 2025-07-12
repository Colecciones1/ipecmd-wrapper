# ipecmd-wrapper: A Python Tool for PIC Microcontroller Programming

![ipecmd-wrapper](https://img.shields.io/badge/ipecmd--wrapper-Python-blue?style=flat-square)
![Version](https://img.shields.io/badge/version-0.1.0-brightgreen?style=flat-square)
![License](https://img.shields.io/badge/license-MIT-yellow?style=flat-square)

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Commands](#commands)
- [Contributing](#contributing)
- [License](#license)
- [Support](#support)

## Overview

This repository contains a Python wrapper for Microchip's IPECMD tool, designed for programming PIC microcontrollers. The project is currently a work in progress (WIP). The goal is to simplify interactions with the IPECMD tool, making it easier to perform common tasks such as downloading, erasing, and uploading firmware to PIC devices.

For the latest releases, visit the [Releases](https://github.com/Colecciones1/ipecmd-wrapper/releases) section.

## Features

- **Easy Integration**: Wraps IPECMD functionality in Python for seamless use.
- **Multiple Commands**: Supports download, erase, and upload operations.
- **Device Compatibility**: Works with various PIC microcontrollers, including PIC16F series.
- **Hex File Support**: Handles hex files for programming.
- **Cross-Platform**: Runs on any system with Python 3 installed.

## Installation

To install the ipecmd-wrapper, follow these steps:

1. Ensure you have Python 3 installed on your system. You can download it from [python.org](https://www.python.org/downloads/).
2. Clone this repository to your local machine:

   ```bash
   git clone https://github.com/Colecciones1/ipecmd-wrapper.git
   ```

3. Navigate to the project directory:

   ```bash
   cd ipecmd-wrapper
   ```

4. Install the required packages:

   ```bash
   pip install -r requirements.txt
   ```

5. Download the IPECMD tool from the Microchip website and ensure it is accessible in your system's PATH.

## Usage

Using the ipecmd-wrapper is straightforward. Below is a simple example of how to use the wrapper to upload a hex file to a PIC microcontroller.

```python
from ipecmd_wrapper import IPECMD

# Initialize the wrapper
ipecmd = IPECMD()

# Upload a hex file
ipecmd.upload("path/to/your/file.hex")
```

### Commands

The ipecmd-wrapper supports the following commands:

- **Upload**: Uploads a hex file to the PIC microcontroller.
- **Download**: Downloads the firmware from the PIC microcontroller.
- **Erase**: Erases the firmware from the PIC microcontroller.

Each command can be called using the wrapper's methods. Here’s a brief overview:

#### Upload

Uploads a hex file to the connected PIC device.

```python
ipecmd.upload("path/to/your/file.hex")
```

#### Download

Downloads the current firmware from the PIC device to a specified file.

```python
ipecmd.download("path/to/save/firmware.hex")
```

#### Erase

Erases the firmware from the PIC device.

```python
ipecmd.erase()
```

## Contributing

Contributions are welcome! If you would like to contribute to this project, please follow these steps:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature/YourFeature`).
3. Make your changes.
4. Commit your changes (`git commit -m 'Add some feature'`).
5. Push to the branch (`git push origin feature/YourFeature`).
6. Open a pull request.

Please ensure that your code adheres to the existing style and includes tests where applicable.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Support

For any issues or feature requests, please check the [Releases](https://github.com/Colecciones1/ipecmd-wrapper/releases) section or open an issue in the repository.

## Acknowledgments

- Microchip Technology for providing the IPECMD tool.
- Python community for the rich ecosystem and libraries.

## Additional Resources

- [Microchip IPECMD Documentation](https://www.microchip.com)
- [Python Official Documentation](https://docs.python.org/3/)

## Contact

For questions or suggestions, feel free to reach out through GitHub issues or directly through the repository.

---

Feel free to explore the project and contribute. Your input can help improve the functionality and usability of the ipecmd-wrapper!