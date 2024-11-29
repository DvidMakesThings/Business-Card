# Business_Card_LA Project

Business_Card_LA is a unique project where a business card doubles as a logic analyzer. It is designed based on Cypress CY7C68013A USB controller. It can sample 8 channels at the same time. The maximum sampling rate of each channel is 24Mhz, and the maximum logical level supports 5.5V. The software adopts sigrok-PulseView, which is open source, and supports Linux, Windows, Mac OS X and other platforms. It supports more than 100 kinds of protocol analysis, and can add its own protocol analysis.

## Specifications
- **Sampling rate and number of channels**: 24Mhz, 8 Channel
- **Signal input range**: 0-5.5V
- **High and low level recognition range**: Vin High: >2V, Vin Low: <0.8V
- **Communication mode**: USB 2.0 (In order to ensure the sampling rate of 24Mhz, try not to use USB docking station)

## Usage
1. **Download sigrok-PulseView Software**: Be sure to download the Release build from [sigrok Downloads](https://sigrok.org/wiki/Downloads).
2. **Install sigrok-PulseView & LogicAnalyzer driver**:
   - After PulseView is installed, run Zadig from the installation folder: `\sigrok\PulseView\zadig.exe`.
   - Select the device you want to install the driver on. The business card appears as Unknown device with VID/PID 04B4:8613.
   - Check Edit, change the device name to fx2LAFw, and then click Install Driver.
3. **Run PulseView**:
   - Click PulseView to run the software.
   - The status LED will light up and it's blue, indicating that the firmware is loaded successfully and the logic signal can be sampled.

## Supported Protocols
See [sigrok Supported Protocol decoders](https://sigrok.org/wiki/Protocol_decoders).

## License
This project is licensed under the GPL-3.0 License.

## Contact
For any questions or feedback, please contact:
- Email: [s.dvid@hotmail.com](mailto:s.dvid@hotmail.com)
- GitHub: [DvidMakesThings](https://github.com/DvidMakesThings)