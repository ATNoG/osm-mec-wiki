---
sidebar_position: 4
---

# Demonstration App

> [Demo App Link Here](https://github.com/PedroDSFerreira/video-object-detection)

![Example Image](./images/demo_app.png)

## Purpose:

This application is used to showcase the onboarding of MEC App.

## Overview:

Object detection client-server application: Server receives a video stream from the client. Using YOLOv3, the server processes the video stream and returns the number of detected objects and their position for each frame.

## Infrastructure:

The application operates within a Containerized Network Function (CNF), which is a form of Virtualized Network Function (VNF). In this setup, the virtualized hardware runs inside a container on its machine.

**Deployment**: The Demo App is containerized using Docker and is managed by Kubernetes, a container orchestration platform. This setup ensures scalability, reliability, and efficient resource utilization.

## More Information:

For detailed documentation and access to the codebase, visit the [GitHub repository](https://github.com/PedroDSFerreira/video-object-detection).