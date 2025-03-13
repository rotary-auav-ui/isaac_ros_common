# Isaac ROS Common

Dockerfiles and scripts for development using the Isaac ROS suite.

## Overview

The [Isaac ROS Common](https://github.com/NVIDIA-ISAAC-ROS/isaac_ros_common)
repository contains a number of scripts and Dockerfiles to help
streamline development and testing with the Isaac ROS suite.

<div align="center"><a class="reference internal image-reference" href="https://media.githubusercontent.com/media/NVIDIA-ISAAC-ROS/.github/main/resources/isaac_ros_docs/repositories_and_packages/isaac_ros_common/isaac_ros_common_tools.png/"><img alt="Isaac ROS DevOps tools" src="https://media.githubusercontent.com/media/NVIDIA-ISAAC-ROS/.github/main/resources/isaac_ros_docs/repositories_and_packages/isaac_ros_common/isaac_ros_common_tools.png/" width="auto"/></a></div>

The Docker images included in this package provide pre-compiled binaries
for ROS 2 Humble on Ubuntu 20.04 Focal.

Additionally, on x86_64 platforms, Docker containers allow you to
quickly set up a sensitive set of frameworks and dependencies to ensure
a smooth experience with Isaac ROS packages. The Dockerfiles for this
platform are based on the version 22.03 image from [Deep Learning
Frameworks Containers](https://docs.nvidia.com/deeplearning/frameworks/support-matrix/index.html).
On Jetson platforms, JetPack manages all of these dependencies for you.

Use of Docker images enables CI|CD systems to scale with DevOps work and
run automated testing in cloud native platforms on Kubernetes.

For solutions to known issues, see the [Troubleshooting](https://nvidia-isaac-ros.github.io/troubleshooting/index.html) section.

---

## Documentation

Please visit the [Isaac ROS Documentation](https://nvidia-isaac-ros.github.io/repositories_and_packages/isaac_ros_common/index.html) to learn how to use this repository.

---

## Quick Installation and Usage (for those who don't want to read the Documentation)

Before using this package, make sure that you've already setup your [Developer Enviroment](https://nvidia-isaac-ros.github.io/v/release-2.1/getting_started/dev_env_setup.html). 

After that you can clone this package to your workspace and run the docker development script. This will mount $ISAAC_ROS_WS defined in your bashrc into the docker container.

Additionally, to configure which docker image to be built, you can add .isaac_ros_common-config file in your scripts folder, additional info on what could be configured is explained in the documentation. 

To add your PX4_Autopilot mountpoint, you can add .px4_mountpoint file in your scripts folder. Currently

---



## Latest

Update 2023-10-18: Updated for Isaac ROS 2.0.0.
