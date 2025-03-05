# NVIDIA Holoscan

[NVIDIA Holoscan](https://developer.nvidia.com/holoscan-sdk) is the AI sensor processing platform that combines hardware systems for low-latency sensor and network connectivity, optimized libraries for data processing and AI, and core microservices to run streaming, imaging, and other applications, from embedded to edge to cloud. It can be used to build streaming AI pipelines for a variety of domains, including Medical Devices, High Performance Computing at the Edge, Industrial Inspection and more.

The Holoscan platform consists of:

## Software

* **Holoscan SDK**: the Software Development Kit
    * [User guide](https://docs.nvidia.com/clara-holoscan/sdk-user-guide/index.html) ([PDF](https://developer.nvidia.com/downloads/holoscan-sdk-user-guide))
    * [Development container](https://catalog.ngc.nvidia.com/orgs/nvidia/teams/clara-holoscan/containers/holoscan)
    * [Debian package](https://catalog.ngc.nvidia.com/orgs/nvidia/teams/clara-holoscan/resources/holoscan_dev_deb)
    * [Python wheel](https://pypi.org/project/holoscan)
    * [Source code](https://github.com/nvidia-holoscan/holoscan-sdk)
* **Holoscan Reference Applications**: community-driven collection of Holoscan reference applications, operators, benchmarks and tutorials
    * [Source code](https://github.com/nvidia-holoscan/holohub)
* **Deployment Software Stack**: OpenEmbedded/Yocto layer for optimized deployment of the Holoscan SDK on the Developer Kits
    * [OpenEmbedded/Yocto Build container](https://catalog.ngc.nvidia.com/orgs/nvidia/teams/clara-holoscan/containers/holoscan-oe-builder)
    * [OpenEmbedded/Yocto Recipes](https://github.com/nvidia-holoscan/meta-tegra-holoscan)
* **Holoscan Sensor Bridge Software**: integrate the Holoscan Sensor Bridge Device in a Holoscan Application
    * [Source code](https://github.com/nvidia-holoscan/holoscan-sensor-bridge)
    * [Documentation](https://docs.nvidia.com/holoscan/sensor-bridge/latest)

## Hardware

### Developer Kits

* [**NVIDIA IGX Orin Developer Kit**](https://www.nvidia.com/en-us/edge-computing/products/igx/) ([User guide](https://github.com/nvidia-holoscan/holoscan-docs/blob/main/devkits/nvidia-igx-orin/nvidia_igx_orin_user_guide.md))
* [**NVIDIA Clara AGX Developer Kit**](https://www.nvidia.com/en-gb/clara/intelligent-medical-instruments/) ([User guide](https://github.com/nvidia-holoscan/holoscan-docs/blob/main/devkits/clara-agx/clara_agx_user_guide.md))
* [**NVIDIA Jetson Orin Developer Kits**](https://www.nvidia.com/en-us/autonomous-machines/embedded-systems/jetson-orin/) ([User Guide](https://developer.nvidia.com/embedded/learn/jetson-agx-orin-devkit-user-guide/index.html))

### Sensors

* [**Holoscan Sensor Bridge Reference Design**](https://www.latticesemi.com/products/developmentboardsandkits/certuspro-nx-sensor-to-ethernet-bridge-board): bring your own sensor, and leverage this FPGA design to send packets over Ethernet, including RDMA support when connected to the ConnectX NIC of a NVIDIA Developer Kit.
* [**AJA Capture Cards**](https://www.aja.com/nav/products-desktop-io): achieve RDMA through these PCIe capture cards using the AJA drivers and Holoscan operator ([Documentation](https://docs.nvidia.com/holoscan/sdk-user-guide/aja_setup.html)/[Operator](https://docs.nvidia.com/holoscan/sdk-user-guide/api/cpp/classholoscan_1_1ops_1_1ajasourceop.html)).
* [**Emergent Vision Tech High-Speed Cameras**](https://emergentvisiontec.com/): achieve RDMA through the ConnectX NIC using the Rivermax SDK and the Emergent Holoscan operator ([Documentation](https://docs.nvidia.com/holoscan/sdk-user-guide/emergent_setup.html)/[Operator](https://github.com/nvidia-holoscan/holohub/tree/main/operators/emergent_source)).

## Additional Tools

* [Holoscan Test Suite](https://github.com/nvidia-holoscan/holoscan-test-suite): support Verification and Validation testing on Holoscan Developer Kits

## Note

In previous releases, the prefix [`Clara`](https://developer.nvidia.com/industries/healthcare) was used to define Holoscan as a platform designed initially for [medical devices](https://www.nvidia.com/en-us/clara/developer-kits/). As Holoscan has grown, its potential to serve other areas has become apparent. Starting with version 0.4.0 of the Holoscan SDK, Holoscan is now officially built to be domain-agnostic and can be used to build sensor AI applications in multiple domains. Going forward, domain specific content will be hosted on the [HoloHub](https://github.com/nvidia-holoscan/holohub) repository.
