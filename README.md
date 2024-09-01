# DruML

DruML is an AI-powered electronic drum module that utilizes convolutional neural networks to predict drum strikes and generate MIDI signals with ultra-low latency. The project is designed to run on STM32 microcontrollers.

## Features

- **Low Latency**: Real-time drum strike prediction and MIDI generation.
- **AI-Driven**: Uses a convolutional neural network for accurate strike classification.
- **Multi-Sensor Input**: Supports multiple piezo sensors for detailed strike detection.
- **Customizable**: Easily adaptable for different sensor configurations and drum setups.

## Requirements

- **Supported STM32 Microcontroller**: Only pre-release alpha hardware is currently supported
- **STM32CubeProgrammer**: Required for flashing the firmware. Download from [STM32CubeProgrammer](https://www.st.com/en/development-tools/stm32cubeprog.html).
- **Hex Files**: Precompiled hex files are available in the [Releases](https://github.com/s0up/druml/releases) section.

## Installation

### Step 1: Download STM32CubeProgrammer

If you haven't already, download and install the STM32CubeProgrammer from the [official website](https://www.st.com/en/development-tools/stm32cubeprog.html).

### Step 2: Flash the Firmware

1. Connect your STM32 Nucleo board to your computer via USB.
2. Open STM32CubeProgrammer.
3. Select the connected device.
4. Navigate to the **Releases** section of this repository and download the appropriate `.hex` file for your device.
5. In STM32CubeProgrammer, go to the **Download** tab, and select the downloaded `.hex` file.
6. Click **Start Programming** to flash the firmware onto your STM32 device.

### Step 3: Connect and Play

Once the firmware is successfully flashed:

1. Connect your drum sensors to the STM32 Nucleo board.
2. Connect the board to your computer or MIDI device.
3. Power on the system and start playing!

## Usage

DruML is designed to work seamlessly with any MIDI-compatible software or hardware. Once connected, it will automatically detect drum strikes and send the corresponding MIDI signals.

## License

This project is currently invite only and closed source.
