# NVIDIA Holoscan

[NVIDIA Holoscan](https://developer.nvidia.com/holoscan-sdk) is the AI sensor processing platform that combines hardware systems for low-latency sensor and network connectivity, optimized libraries for data processing and AI, and core microservices to run streaming, imaging, and other applications, from embedded to edge to cloud. It can be used to build streaming AI pipelines for a variety of domains, including Medical Devices, High Performance Computing at the Edge, Industrial Inspection and more.

> In previous releases, the prefix [`Clara`](https://developer.nvidia.com/industries/healthcare) was used to define Holoscan as a platform designed initially for [medical devices](https://www.nvidia.com/en-us/clara/developer-kits/). As Holoscan has grown, its potential to serve other areas has become apparent. With version 0.4.0 of the Holoscan SDK, we're proud to announce that Holoscan is now officially built to be domain-agnostic and can be used to build sensor AI applications in multiple domains. Going forward, domain specific content will be hosted on the [HoloHub](https://github.com/nvidia-holoscan/holohub) repository.

The Holoscan platform consists of:

## Holoscan Software

* **Holoscan SDK**: the Development Kit
    * [User guide](https://docs.nvidia.com/clara-holoscan/sdk-user-guide/index.html) ([PDF](https://developer.nvidia.com/downloads/holoscan-sdk-user-guide))
    * [Development container](https://catalog.ngc.nvidia.com/orgs/nvidia/teams/clara-holoscan/containers/holoscan)
    * [Debian package](https://catalog.ngc.nvidia.com/orgs/nvidia/teams/clara-holoscan/resources/holoscan_dev_deb)
    * [Python wheel](https://pypi.org/project/holoscan)
    * [Source code](https://github.com/nvidia-holoscan/holoscan-sdk)
* **HoloHub**: community-driven collection of Holoscan applications, operators, and tutorials
    * [Website](https://nvidia-holoscan.github.io/holohub)
    * [Source code](https://github.com/nvidia-holoscan/holohub)
* **Deployment Software Stack**: OpenEmbedded/Yocto layer for optimized deployment of the Holoscan SDK on the Developer Kits
    * [OpenEmbedded/Yocto Build container](https://catalog.ngc.nvidia.com/orgs/nvidia/teams/clara-holoscan/containers/holoscan-oe-builder)
    * [OpenEmbedded/Yocto Recipes](https://github.com/nvidia-holoscan/meta-tegra-holoscan)

## Developer Kits

* **[NVIDIA Clara AGX Developer Kit](https://www.nvidia.com/en-gb/clara/intelligent-medical-instruments/)**
    * Jetson AGX Xavier™, RTX™ 6000 GPU, ConnectX® SmartNIC
    * [User guide](https://github.com/nvidia-holoscan/holoscan-docs/blob/main/devkits/clara-agx/clara_agx_user_guide.md)
* **[NVIDIA IGX Orin Developer Kit](https://www.nvidia.com/en-us/edge-computing/products/igx/)**
    * Jetson AGX Orin™, RTX™ A6000 GPU, ConnectX® SmartNIC
    * [User guide](https://github.com/nvidia-holoscan/holoscan-docs/blob/main/devkits/nvidia-igx-orin/nvidia_igx_orin_user_guide.md)

## Additional Tools

* [Holoscan Test Suite](https://github.com/nvidia-holoscan/holoscan-test-suite): support Verification and Validation testing on Holoscan Developer Kits
* [Holoscan Perf Tools](https://github.com/nvidia-holoscan/holoscan-perf-tools): collection of tools to help measure performance of the Holoscan platform (software and hardware)
* [L4T Compute Assist](https://catalog.ngc.nvidia.com/orgs/nvidia/teams/clara-holoscan/containers/l4t-compute-assist): utility container to perform computation on the integrated GPU (iGPU) of Holoscan Developer Kits configured to use their discrete GPU (dGPU)
