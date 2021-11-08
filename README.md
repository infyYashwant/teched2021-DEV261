# DEV261 - Build Extensions with SAP BTP, Kyma Runtime

<img src="kyma-runtime.svg" width="300">

## Description

This repository contains the material for the SAP TechEd 2021 session called DEV261 - "Build Extensions with SAP BTP, Kyma Runtime".

## Overview

This session introduces attendees to making use of the advantages that come along with Kubernetes in the context of their SAP BTP projects. SAP BTP, Kyma runtime is the fully managed Kubernetes runtime based on the open-source project "Kyma". This cloud-native solution allows the developers to extend SAP solutions with serverless Functions and combine them with containerized microservices. The offered functionality ensures smooth consumption of SAP and non-SAP applications, running workloads in a highly scalable environment, and building event- and API-based extensions.

During this session, you will learn how to make use of SAP BTP services in the context of a Kyma-based project. You will see how to

- setup your continous integration and delivery pipeline using "[SAP Continuous Integration and Delivery](https://discovery-center.cloud.sap/serviceCatalog/continuous-integration-&-delivery)" for deploying a CAP application. This application will also make use of the services:
  - [SAP Launchpad service](https://discovery-center.cloud.sap/serviceCatalog/launchpad-service),
  - [SAP HANA Cloud](https://discovery-center.cloud.sap/serviceCatalog/sap-hana-cloud)
  - [SAP Alert Notification](https://discovery-center.cloud.sap/serviceCatalog/alert-notification)
  - [SAP HTML5 Application Repository](https://discovery-center.cloud.sap/serviceCatalog/html5-application-repository-service)

## Requirements

To follow the exercises in this repository, you need to have a free SAP BTP trial account or you make use of the free tier inside your SAP BTP global account. Details are described on [SAP.com](https://www.sap.com/products/business-technology-platform/trial.html).

Furthermore, you need to have the following tools and frameworks installed on your computer:

- [kubectl](https://developers.sap.com/tutorials/cp-kyma-download-cli.html)
- [nodejs version 14.\*](https://nodejs.org/en/download/)
- [jq](https://stedolan.github.io/jq/) - for JSON processing in CLI
- [Docker Desktop](https://www.docker.com/) installed with a valid public account
  > Be aware of the terms of Docker for usage in enterprises. For details see [link](https://www.docker.com/blog/updating-product-subscriptions/)

## Exercises

Provide the exercise content here directly in README.md using [markdown](https://guides.github.com/features/mastering-markdown/) and linking to the specific exercise pages, below is an example.

- [Getting Started](exercises/ex0/)
  - [FORK AND CLONE REPO](https://github.com/SAP-samples/teched2021-DEV261/blob/main/exercises/ex0/README.md#configure-subaccount-entitlements)
  - [SAP BTP SUBACCOUNT CONFIGURATION](https://github.com/SAP-samples/teched2021-DEV261/blob/main/exercises/ex0/README.md#kyma-runtime)
  - [SAP KYMA RUNTIME](https://github.com/SAP-samples/teched2021-DEV261/blob/main/exercises/ex0/README.md#launchpad-service)
    - [PROVISIONING](https://github.com/SAP-samples/teched2021-DEV261/blob/main/exercises/ex0/README.md#launchpad-service)
    - [ROLE ASSIGNMENT](https://github.com/SAP-samples/teched2021-DEV261/blob/main/exercises/ex0/README.md#cloud-foundry)
    - [KUBECTL CONFIGURATION](https://github.com/SAP-samples/teched2021-DEV261/blob/main/exercises/ex0/README.md#sap-hana-cloud)
  - [SAP LAUNCHPAD SERVICES](https://github.com/SAP-samples/teched2021-DEV261/blob/main/exercises/ex0/README.md#sap-hana-cloud)
    - [PROVISIONING](https://github.com/SAP-samples/teched2021-DEV261/blob/main/exercises/ex0/README.md#sap-hana-cloud)
    - [ROLE ASSIGNMENT](https://github.com/SAP-samples/teched2021-DEV261/blob/main/exercises/ex0/README.md#sap-hana-cloud)
  - [SAP CLOUD FOUNDRY CONFIGURATION](https://github.com/SAP-samples/teched2021-DEV261/blob/main/exercises/ex0/README.md#sap-hana-cloud)
  - [SAP CICD SERVICE](https://github.com/SAP-samples/teched2021-DEV261/blob/main/exercises/ex0/README.md#sap-hana-cloud)
    - [PROVISIONING](https://github.com/SAP-samples/teched2021-DEV261/blob/main/exercises/ex0/README.md#sap-hana-cloud)
    - [ROLE ASSIGNMENT](https://github.com/SAP-samples/teched2021-DEV261/blob/main/exercises/ex0/README.md#sap-hana-cloud)
  - [SAP HANA CLOUD](https://github.com/SAP-samples/teched2021-DEV261/blob/main/exercises/ex0/README.md#sap-hana-cloud)
    - [PROVISIONING](https://github.com/SAP-samples/teched2021-DEV261/blob/main/exercises/ex0/README.md#sap-hana-cloud)
    - [CONFIGURATION](https://github.com/SAP-samples/teched2021-DEV261/blob/main/exercises/ex0/README.md#sap-hana-cloud)
- [Exercise 1 - CREATE THE XSUAA SERVICE INSTANCE](exercises/ex1/)
- [Exercise 2 - PREPARE APP FOR LOCAL USE](exercises/ex2/)
- [Exercise 3 - CONFIGURE THE SAP CICD SERVICE](exercises/ex3/)
  - [Exercise 3.1 - CREATE THE GITHUB CREDENTIAL](exercises/ex3#exercise-31---create-the-github-credential)
  - [Exercise 3.2 - CREATE THE DOCKER CREDENTIAL](exercises/ex3#exercise-32---create-the-docker-credential)
  - [Exercise 3.3 - CONFIGURE KUBECONFIG](exercises/ex3#exercise-33---configure-kubeconfig)
  - [Exercise 3.4 - ADD THE GITHUB REPOSITORY](exercises/ex3#exercise-34---add-the-github-repository)
  - [Exercise 3.5 - CREATE THE CICD JOBS](exercises/ex3#exercise-35---create-the-cicd-jobs)
    - [Exercise 3.5.1 - CAP-ORDERS-SERVICE](exercises/ex3#exercise-351---cap-orders-service)
    - [Exercise 3.5.2 - ORDERS-HTML5-DEPLOYER - OPTIONAL](exercises/ex3#exercise-352---orders-html5-deployer---optional)
    - [Exercise 3.5.3 - ORDERS-DB-DEPLOYER- OPTIONAL](exercises/ex3#exercise-353---orders-db-deployer---optional)
    - [Exercise 3.5.4 - CAPUITOOLS - OPTIONAL](exercises/ex3#exercise-354---capuitools---optional)
- [Exercise 4 - GENERATE TOOLS BASE IMAGE](exercises/ex2/)
- [Exercise 5 - GENERATE THE CAP DATABASE](exercises/ex2/)
  - [Exercise 5.1 - DEPLOYMENT OPTION 1 - kubectl]()
  - [Exercise 5.2 - DEPLOYMENT OPTION 2 - Helm]()
  - [Exercise 5.3 - DEPLOYMENT OPTION 3 - Local Deployment]()
  - [Exercise 5.4 - LOCALLY RUNNING THE APPLICATION]()
- [Exercise 6 - DEPLOY HTML5 APP AND LAUNCHPAD CONFIG ](exercises/ex2/)
  - [Exercise 6.1 - DEPLOYMENT OPTION 1 - kubectl]()
  - [Exercise 6.2 - DEPLOYMENT OPTION 2 - Helm]()
- [Exercise 7 - BUILD AND DEPLOY CAP SERVICE](exercises/ex2/)
  - [Exercise 7.1 - CONFIGURE HELM CHART]()
  - [Exercise 7.2 - DEPLOYMENT OPTION 1 - SAP CICD]()
  - [Exercise 7.3 - DEPLOYMENT OPTION 2 - kubectl]()
  - [Exercise 7.3 - DEPLOYMENT OPTION 2 - Helm]()
- [Exercise 8 - CONFIGURE LAUNCHPAD](exercises/ex2/)
- [Exercise 9 - REQUIRE OAUTH FOR THE ACTION](exercises/ex2/)
- [Exercise 10 - SAP ALERT NOTIFICATION CONFIGURATION](exercises/ex2/)
- [Exercise 11 - MOCK APPLICATION](exercises/ex2/)
  - [Exercise 11.1 - KYMA SERVERLESS FUNCTION]()

**OR** Link to the Tutorial Navigator for example...

Start the exercises [here](https://developers.sap.com/tutorials/abap-environment-trial-onboarding.html).

**IMPORTANT**

Your repo must contain the .reuse and LICENSES folder and the License section below. DO NOT REMOVE the section or folders/files. Also, remove all unused template assets(images, folders, etc) from the exercises folder.

## How to obtain support

Support for the content in this repository is available during the actual time of the online session for which this content has been designed. Otherwise, you may request support via the [Issues](../../issues) tab.

## License

Copyright (c) 2021 SAP SE or an SAP affiliate company. All rights reserved. This project is licensed under the Apache Software License, version 2.0 except as noted otherwise in the [LICENSE](LICENSES/Apache-2.0.txt) file.
