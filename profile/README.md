# NVIDIA Holoscan

[NVIDIA Holoscan](https://developer.nvidia.com/holoscan-sdk) is the AI sensor processing platform that combines hardware systems for low-latency sensor and network connectivity, optimized libraries for data processing and AI, and core microservices to run streaming, imaging, and other applications, from embedded to edge to cloud. It can be used to build streaming AI pipelines for a variety of domains, including Medical Devices, High Performance Computing at the Edge, Industrial Inspection, Robotics, and more.

The Holoscan platform consists of:

## Software

* **Holoscan Reference Applications**: community-driven collection of Holoscan reference applications, operators, benchmarks and tutorials
    * [Catalog](https://nvidia-holoscan.github.io/holohub/)
    * [Source code](https://github.com/nvidia-holoscan/holohub)
* **Holoscan SDK**: the Software Development Kit
    * [User guide](https://docs.nvidia.com/clara-holoscan/sdk-user-guide/index.html) ([PDF](https://developer.nvidia.com/downloads/holoscan-sdk-user-guide))
    * [Development container](https://catalog.ngc.nvidia.com/orgs/nvidia/teams/clara-holoscan/containers/holoscan)
    * [Debian package](https://catalog.ngc.nvidia.com/orgs/nvidia/teams/clara-holoscan/resources/holoscan_dev_deb)
    * [Python wheel](https://pypi.org/project/holoscan)
    * [Source code](https://github.com/nvidia-holoscan/holoscan-sdk)
* **Holoscan Deployment Stack**: OpenEmbedded/Yocto layer for optimized deployment of applications developed using the Holoscan SDK
    * [OpenEmbedded/Yocto Build container](https://catalog.ngc.nvidia.com/orgs/nvidia/teams/clara-holoscan/containers/holoscan-oe-builder)
    * [OpenEmbedded/Yocto Recipes](https://github.com/nvidia-holoscan/meta-tegra-holoscan)
* **Holoscan Sensor Bridge Software**: integrate the Holoscan Sensor Bridge Device in a Holoscan Application
    * [Source code](https://github.com/nvidia-holoscan/holoscan-sensor-bridge)
    * [Documentation](https://docs.nvidia.com/holoscan/sensor-bridge/latest)

## Software Support
* **Long Term Support**: critical bug fixes and patches for high/critical software vulnerabilities, with guaranteed API stability
    * [Latest LTSB 10-Year Support Branch](https://catalog.ngc.nvidia.com/orgs/nvidia/collections/long_term_support_branch_2_igx)
    * [Latest Production Branch 9-months support](https://catalog.ngc.nvidia.com/orgs/nvidia/collections/production_branch_october_2024)

## Hardware

### Developer Kits

* [**NVIDIA Jetson Orin Nano (Super) Developer Kits**](https://developer.nvidia.com/embedded/learn/get-started-jetson-orin-nano-devkit) ([User Guide](https://developer.nvidia.com/embedded/learn/jetson-orin-nano-devkit-user-guide/index.html))
* [**NVIDIA Jetson AGX Orin Developer Kits**](https://developer.nvidia.com/embedded/learn/get-started-jetson-agx-orin-devkit) ([User Guide](https://developer.nvidia.com/embedded/learn/jetson-agx-orin-devkit-user-guide/index.html))
* [**NVIDIA IGX Orin Developer Kit**](https://www.nvidia.com/en-us/edge-computing/products/igx/) ([User guide](https://github.com/nvidia-holoscan/holoscan-docs/blob/main/devkits/nvidia-igx-orin/nvidia_igx_orin_user_guide.md))
* [**NVIDIA Clara AGX Developer Kit**](https://www.nvidia.com/en-gb/clara/intelligent-medical-instruments/) ([User guide](https://github.com/nvidia-holoscan/holoscan-docs/blob/main/devkits/clara-agx/clara_agx_user_guide.md))
* x86 PC or Laptop with supported Nvidia GPUs (Ampere and above)

### Sensor Interfaces

* **Holoscan Sensor Bridge Reference Design and DevKits**: bring your own sensor, and leverage this FPGA design to send packets over Ethernet (including RDMA support if connected to the ConnectX NIC).
   * [CertusPro-NX Sensor to Ethernet Bridge Board](https://www.latticesemi.com/products/developmentboardsandkits/certuspro-nx-sensor-to-ethernet-bridge-board)
   * [PolarFire® FPGA Ethernet Sensor Bridge](https://www.microchip.com/en-us/products/fpgas-and-plds/boards-and-kits/ethernet-sensor-bridge)
* **PCIe Sensor I/O Cards**: transfer data in an out of Nvidia GPUs using supported PCIe cards from partners (using GPUDirect RDMA if installed on NVIDIA IGX).
   * [**AJA Capture Cards**](https://www.aja.com/nav/products-desktop-io): achieve GPUDirect RDMA through these PCIe capture cards using the AJA drivers and Holoscan operator ([Documentation](https://docs.nvidia.com/holoscan/sdk-user-guide/aja_setup.html)/[Operator](https://docs.nvidia.com/holoscan/sdk-user-guide/api/cpp/classholoscan_1_1ops_1_1ajasourceop.html)).
   * [**Deltacast Capture Cards**](https://www.deltacast.tv/products/developer-products): achieve GPUDirect RDMA through these PCIe capture cards ([Reference application](https://nvidia-holoscan.github.io/holohub/applications/deltacast_transmitter/?h=deltacast))

## Additional Tools

* [Holoscan Test Suite](https://github.com/nvidia-holoscan/holoscan-test-suite): support Verification and Validation testing on Holoscan Developer Kits

## Note

In previous releases, the prefix [`Clara`](https://developer.nvidia.com/industries/healthcare) was used to define Holoscan as a platform designed initially for [medical devices](https://www.nvidia.com/en-us/clara/developer-kits/). As Holoscan has grown, its potential to serve other areas has become apparent. Starting with version 0.4.0 of the Holoscan SDK, Holoscan is now officially built to be domain-agnostic and can be used to build sensor AI applications in multiple domains. Going forward, domain specific content will be hosted on the [HoloHub](https://github.com/nvidia-holoscan/holohub) repository.
