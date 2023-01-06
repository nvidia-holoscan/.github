# NVIDIA Holoscan

__NVIDIA Holoscan__ is the AI sensor processing platform that combines hardware systems for low-latency sensor and network connectivity, optimized libraries for data processing and AI, and core microservices to run streaming, imaging, and other applications, from embedded to edge to cloud. It can be used to build streaming AI pipelines for a variety of domains, including Medical Devices, High Performance Computing at the Edge, Industrial Inspection and more.

> In previous releases, the prefix [`Clara`](https://developer.nvidia.com/industries/healthcare) was used to define Holoscan as a platform designed initially for [medical devices](https://www.nvidia.com/en-us/clara/developer-kits/). As Holoscan has grown, its potential to serve other areas has become apparent. With version 0.4.0 of the Holoscan SDK, we're proud to announce that Holoscan is now officially built to be domain-agnostic and can be used to build sensor AI applications in multiple domains. Going forward, domain specific content will be hosted on the [HoloHub](https://github.com/nvidia-holoscan/holohub) repository.

Holoscan consists of:

## Holoscan Software
* **Holoscan SDK**
    * [User guide](https://docs.nvidia.com/clara-holoscan/sdk-user-guide/index.html)
    * [Source code](https://github.com/nvidia-holoscan/holoscan-sdk)
    * [Python Wheel](https://pypi.org/project/holoscan/)
    * [NGC collection: containers and binaries](https://catalog.ngc.nvidia.com/orgs/nvidia/teams/clara-holoscan/collections/clara_holoscan)
* **HoloHub**
    * [Source code](https://github.com/nvidia-holoscan/holohub)
* **Deployment Software Stack**
    * [Holoscan OpenEmbedded/Yocto recipes](https://github.com/nvidia-holoscan/meta-tegra-holoscan)
    * [Holoscan OpenEmbedded/Yocto build container](https://catalog.ngc.nvidia.com/orgs/nvidia/teams/clara-holoscan/containers/holoscan-oe-builder)

## Holoscan Developer Kits
* **NVIDIA Clara AGX Developer Kit** (Jetson AGX Xavier™, RTX™ 6000 GPU, ConnectX® SmartNIC)
* **NVIDIA IGX Orin Developer Kit** (AGX Orin™, RTX™ A6000 GPU, ConnectX® SmartNIC)

## Performance Tools
Collection of tools to help measure performance of the Holoscan platform (software and hardware).
* [Holoscan Perf Tools](https://github.com/nvidia-holoscan/holoscan-perf-tools)

Visit the [NVIDIA Developer Page](https://developer.nvidia.com/clara-holoscan-sdk) to learn more about Holoscan and get started today.
