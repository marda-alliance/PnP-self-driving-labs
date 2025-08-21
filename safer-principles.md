# The “SAFER” Guiding Principles to Enable Plug-and-Play Tools for Autonomous Laboratories

The FAIR Guiding Principles for scientific data management and stewardship, introduced in 2016, emphasize the importance of ensuring data is Findable, Accessible, Interoperable, and Reusable (FAIR). These principles have provided a widely recognized framework for improving the machine-actionability and sharing of digital data, fostering collaboration and innovation across disciplines. Inspired by the success of FAIR, the SAFER Guiding Principles—Standardization, Automation, Flexibility, Ease of Use, and Resiliency—are introduced as a framework for defining and evaluating plug-and-play capabilities and maturity within the cyber-physical infrastructure supporting autonomous and automated laboratories. SAFER principles aim to ensure that software, hardware, devices, systems, and technologies in interconnected environments are seamlessly integrated, widely compatible, and user-friendly, enabling efficient and reliable operation without requiring extensive configuration or technical expertise. These guiding principles provide a foundation for advancing plug-and-play functionality to support the growing complexity and connectivity in autonomous and automated laboratories.

## Standardization

- Devices and systems should support widely accepted standards for mechanical interfaces, programmatic interfaces, communication protocols, and data exchange formats.
- Devices and systems should be backward compatible with past systems and attempt to be prepared for forward compatibility with next-generation systems.
- Devices, systems, software, and components should describe their features and functions using a machine-actionable language.
- When specific standards do not exist, devices, systems, software, and components should default to open and machine-actionable formats (e.g., JSON, XML, HDF5, CSV, etc.), and communicate the underlying semantics/structure in machine-actionable formats (e.g., OpenAPI, XML/JSON schemas, data dictionaries, etc.).

## Automation

- The process of recognizing, configuring, and enabling a device or system should be automated without requiring significant manual intervention.
- Systems should support automatic driver installation, self-testing, and diagnostics to streamline setup and ensure functionality.
- Systems should safeguard critical functionality by enforcing input invariants with thorough unit testing. 
- Systems should report the results of a combination of qualitative and quantitative checks for either software packages or hardware. 
  - For hardware, this would include an automated self-calibration test and validation. 
  - For software, this would be a complete unit test of all functions and methods. 
- Systems should support discovery on a network, without the need for a registry service, by listening for requests for certain features/capabilities on the network (e.g., query - who can perform an XRD characterization for a certain sample geometry).

## Flexibility

- Plug-and-play systems should be flexible enough to operate in diverse environments and accommodate a range of use cases.
- Devices should support hot-swapping, allowing them to be added, removed, or replaced without disrupting the system or requiring a reboot.
- Devices should be adaptable to work seamlessly with both older (legacy) systems and newer (modern) technologies. 
- Devices with standardized interfaces should accept mechanical and digital connectivity to devices supplied by other vendors (i.e., there should be no vendor lock-in). 

## Ease of Use

- Plug-and-play systems must prioritize user-friendliness, enabling non-technical users to connect and use devices with minimal effort.
- Installation and configuration processes should be intuitive, requiring no specialized knowledge or training.
- Plug-in-play systems must be designed with minimal, efficient dependencies, with a particular avoidance of outdated, unmaintained, or poorly documented packages. 
- Systems should provide clear feedback to users, such as confirming successful connections or diagnosing issues with minimal complexity.
- Software should be packaged/containerized or readily packagable/containerizable.
- Software, systems, and components should be sufficiently labeled so as to facilitate humans in looking up documentation and other resources. 
- Systems should include human-readable descriptions of high-level architecture and data flows, including graphical maps (flow chart, etc.)

## Resiliency

- Software and Hardware should run consistently for an extended period without needing constant supervision or frequent calibration.
- Automatically attempt connectivity in case of network outage or power outage or a disconnect of devices without needing a full reboot.
- Instruments should automate diagnostics and calibration methods to minimize technician intervention.
- Hardware should shutdown gracefully in event of safety stop or device failure, communicating the source of the interruption and offering automatic restart and reconnection if can be done so safely.
- Systems and software should have the capability to send immediate alerts to emergency contacts to minimize harm during failure modes. 
- Software should be sufficiently decoupled from operating systems such that operating systems can be patched/upgraded and kept secure.

## Case Study Ideas

### Instrumentation/Hardware:

- LEGOLAS kit
- Keithley Source Meter
- Camera controller for TEM?
  - https://directelectron.com/de-16/
  - https://github.com/directelectron/deapi
- Profilometer or Laser-Indenter or Laser-engraver in AIMD?

### Software Packages:

- Sci-Kit Learn (Best case scenario)
- Github package provided by a random paper (I’ll volunteer my own repo)
  - https://github.com/hollejd1/logicalEELS
- Deploy on various hardware? Windows PC, Mac ARM64? 
- OpenMSIStream

## Various Links

- https://oshwa.org/ 
- https://sila-standard.com/
- https://opcfoundation.org/about/opc-technologies/opc-ua/
- https://mqtt.org/
- https://sila-standard.com/
- https://www.go-fair.org/fair-principles/
- https://www.w3.org/submissions/OWL-S/
- https://www.ivifoundation.org/getting-started/
- https://link.springer.com/article/10.1557/s43577-022-00430-2
- https://www.agilent.com/en/service/software-for-lab-management/core-facilities-management-software-ilab



