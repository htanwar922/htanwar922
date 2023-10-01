- 👋 Hi, I’m Himanshu.
- 👀 I’m interested in SDN and IoT.
- 🌱 I’m currently learning networking, high-level and low-level design.
- 💞️ I’m looking to collaborate on SDN, Embedded Systems, DLMS/COSEM smart meters.
- 📫 Reach me via:
  - [Gmail](mailto:htanwar922@gmail.com)
  - [IITR Webmail](mailto:himanshu@ee.iitr.ac.in)
  - [IITD Webmail](mailto:Himanshu@ee.iitd.ac.in)
  - [LinkedIn](https://www.linkedin.com/in/htanwar922/).

<!---
htanwar922/htanwar922 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->

<br>

# Academic Qualifications
## Indian Institute of Technology Delhi
### Master of Science (Research) - Electrical Engineering (2021-2023)
CGPA - 8.143/10 \
Projects:
- DLMS/COSEM implementation on following platforms:
  - Linux (Ubuntu, RaspberryPi)
  - STM32F207ZG
- MERN website for displaying smart meters data.
- DLMS-Wireshark for displaying expanded (array and structure in) DLMS _normal_ packets in Wireshark.
- SDN TCP SYN flood detection and mitigation (ongoing).
<hr>

## Indian Institute of Technology Roorkee
### Bachelor of Technology - Electrical Engineering (2017-2021)
CGPA - 8.383/10 \
Projects:
- FPGA-based implementation of Numerical Overcurrent relay.
- Industry-Oriented Project: Apportionate Battery-Capacitor (ABC) for Electric Vehicles.
- B.Tech. Project: 3D real-time mapping using Kinect v2 vision sensor in ROS environment.
<hr>

## CBSE X+2 and Matriculation
### X+2 (Non-Medical)
- Percentage - 93.8%
### Matriculation
- CGPA - 9.6/10

<br>

# Experience
## Samsung Research Institute, Noida
### Internship (May 2020 - June 2020)
Projects:
- Cross-lingual text classification
<hr>

## IIT Roorkee Motorsports
### Vehicle Control Unit Engineer
Projects:
- Vehicle Control Unit (VCU) for Formula Student race car for Formula Green 2020 competition.

<br>

# Projects
## DLMS/COSEM
- [DLMS/COSEM implementation on Linux (Ubuntu, RaspberryPi)][DLMS-COSEM]
  - Implemented Register class in fork from [EPRI:DLMS/COSEM] in collaboration with [github:sudeshna]
  - Implemented a Data Compression algorithm in Python and integrated with the inter-host DLMS/COSEM communication using TCP/IP and shared memory approaches for inter-process communication.
  - Implemented the Data Compression algorithm in C/C++ using TNT Matrix libraries. This allowed implementation of the complete application in C/C++ completely, and a seamless transition of the algorithm to STM32 implementation later on.
  - Deployed 10 RaspberryPi-based DLMS/COSEM-enabled smart meters around IIT Delhi campus.
  - Deployed a DLMS/COSEM-enabled Head-End System on Linux VMs hosted on IIT Delhi Cloud - _Baadal_ - for collecting data from the meters at r intervals and store in MongoDB database.
- [DLMS/COSEM implementation on STM32F207ZG][DLMS-COSEM_STM32]
  - Modified Linux libmodbus library to integrate to STM32 application, exposing read, write and delay functions for custom handling of modbus requests/responses.
  - Implemented ESP8266 libraries in two different ways to integrate with multi-threaded STM32 DLMS/COSEM application in collaboration with [github:venus696].
- [MERN website for displaying smart meters data][IoT-Cloud]
  - Hosted on Linux VMs on IIT Delhi Cloud - _Baadal_ - accessible over IITD intranet for displaying data collected from the deployed smart meters.
  - The website is written for two projects - Air Pollution Monitoring Device (APMD) and Smart Meters (SM).
  - The website allows selecting a date-range or a rolling-plot option, and desired metrics from a list of available metrics.
  - OpenLayers used to render a map of IIT Delhi with an additional layer with overlays to show checkboxes with location-popups marking locations of the installed smart meters around the campus.
- [DLMS-Wireshark for displaying expanded (array and structure in) DLMS _normal_ packets in Wireshark][DLMS-Wireshark]
  - Modified fork from [matousp:dlms-analysis] github repository in lua to expand and display the COSEM structure and array (ASN.1 format) DLMS _normal_ packets in Wireshark.

[DLMS-COSEM]: https://github.com/sudeshna1816/DLMS-COSEM.git
[DLMS-COSEM_STM32]: https://github.com/htanwar922/DLMS-COSEM_STM32.git
[IoT-Cloud]: https://github.com/htanwar922/IoT-CLoud.git
[DLMS-Wireshark]: https://github.com/htanwar922/DLMS-Wireshark.git
[EPRI:DLMS/COSEM]: https://github.com/epri-dev/DLMS-COSEM.git
[matousp:dlms-analysis]: https://github.com/matousp/dlms-analysis
[github:sudeshna]: https://github.com/sudeshna1816
[github:venus696]: https://github.com/venus696

## Vehicle Control Unit
- Developed Vehicle Control Unit (VCU) for Formula Student Electric race car as per Formula Green 2020 rule-book:
  - Shutdown circuit to control and cut power supply from battery to motor controller (and motor).
  - Several PCBs (schematic and layout design, and soldering) to control the shutdown circuit.
  - Programming STM32F103RB controller for algorithms to implement some controls in and out of rule-book.
  - SPI communication of the STM32 board with an ADC and an nRF24L01+ board.

## Cross-lingual text classification
- Sentiment classification for a target language for which only small amounts of labelled data is available using transfer learning on a source language for which large datasets for the same are available:
  - Sentiment classification training of base layers of the Adversarial Network model on source language datasets.
  - Adversarial training with language detector branch of the Adversarial Network model.
- The model was implemented on Tensorflow-Keras framework for Amazon reviews dataset with English as source language and French as target language.
