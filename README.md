A Home Assistant integration to control HyperHDR LED controller. This integration provides switches to control the LED and USB capture devices, a brightness slider, and buttons to activate various effects.

## Features

### Controls
- **LED Output Switch**: Turn the LED strip on/off
- **USB Capture Switch**: Control the USB capture device
- **Brightness Slider**: Adjust LED brightness from 0-100%

### Effects
Buttons to activate various effects including:
- Atomic Swirl
- Blue mood blobs
- Breath
- Candle
- Cinema brighten/dim lights
- Cold mood blobs
- Double swirl
- Full color mood blobs
- Green mood blobs
- Knight rider
- Notify Blue
- Plasma
- Police lights (single/solid)
- Rainbow swirl (normal/fast)
- Rainbow waves
- Red mood blobs
- Sea waves
- Sparks
- Strobe (red/white)
- System shutdown
- Warm mood blobs
- Waves with color

## Installation

### HACS (Recommended)

1. Open HACS in your Home Assistant instance
2. Click on "Integrations"
3. Click the three dots in the top right corner
4. Select "Custom repositories"
5. Add this repository URL and select "Integration" as the category
6. Click "Add"
7. Search for "HyperHDR Control" in HACS
8. Click "Download"
9. Restart Home Assistant

### Manual Installation

1. Copy the `custom_components/hyperhdr_control` directory to your Home Assistant's `custom_components` directory
2. Restart Home Assistant

## Configuration

### Automatic Discovery
The integration will automatically discover HyperHDR instances on your network using zeroconf.

### Manual Setup
1. Go to Settings → Devices & Services
2. Click "Add Integration"
3. Search for "HyperHDR Control"
4. Enter your HyperHDR server's IP address and port (default: 8090)

## Usage

### LED Control
- Use the "HyperHDR LED Output" switch to turn the LED strip on or off
- Use the "HyperHDR USB Capture" switch to control the USB capture device
- Adjust the "HyperHDR Brightness" slider to control LED brightness (0-100%)

### Effects
- Each effect is available as a button in Home Assistant
- Press any effect button to activate that effect
- Effects will run indefinitely until another effect is activated or the LED output is turned off

### Automations
All entities can be used in automations. Examples:
- Turn on LED strip at sunset
- Activate specific effects at certain times
- Adjust brightness based on time of day
- Turn on USB capture when watching TV

## Support

If you encounter any issues or have suggestions:
1. Check the debug logs if you encounter any problems
2. Open an issue on GitHub with:
   - Description of the problem
   - Debug logs if applicable
   - Steps to reproduce the issue 
