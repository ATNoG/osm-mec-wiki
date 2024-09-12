---
sidebar_position: 2
---

# Infrastructure

## Project Goals

- Create a CFS Portal enabling the instantiation, termination and monitoring of MEC Apps.

- Develop an MEC Application Orchestrator capable of deploying MEC Apps as VNFs through OSM platform.

- Create a video processing application to showcase the project's functionalities.

## Architecture

[Project Diagram](./images/infrastructure.png)

### CFS Portal

The CFS Portal is the UI for interacting with the system.

- Dashboard: Overview of the system

- App Catalog: View and create MEC Apps

- MEC Instances: View and update instantiated MEC Apps

- VIM Accounts: View and create VIM Accounts

### OSS

The Operations Support System is responsible for redirecting the user requests to MEAO.

### MEAO
The MEC Application Orchestrator is responsible for:

- Instantiating, updating, and terminating MEC Apps.

- Deploying MEC Apps as VNFs.

- Monotoring MEC Apps.

## Interaction Between Components

### API

The API enables communication between the CFS Portal and OSS, as well as allowing users to make requests directly to the API instead of using the CFS Portal.

### Kafka

Kafka enables communication between OSS and MEAO.

The Kafka topics available are:
- new_app_pkg
- instantiate_app_pkg
- update_app_pkg
- terminate_app_pkg
- delete_app_pkg
- responses

### MongoDB

Mongo Database is used to storage of file descriptors.

Document fields are:

- app_id
- name
- provider
- version
- mec-version
- info-name
- description
- appd
- ns_pkg_id
- vnf_pkg_id