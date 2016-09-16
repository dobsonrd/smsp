---
title: SMSP Assurance Overview
keywords: reference
summary: "SMSP Assurance Overview"
sidebar: mydoc_sidebar
permalink: smsp_assurance_overview.html
folder: smsp
toc: false
---

## SMSP Assurance Overview

Through the following two scenarios of the outline of assurance is explained.

## Scenario 1 - New App Supplier with no customer
Acme Online are developing a new online application providing clinical workflow management for health care professional, they would like to compare the local demographics (Patient Name, DOB, NHS Number, Address, Sex, Registered GP) with the NHS Digital Demographics system, and provide the clinician with the opportunity to update the local held data.

Their intended customers are mainly NHS healthcare trusts.

Currently they have no firm customers, but are confident they have a viable product and would like to progress development. 

Acme Online are aware they need to be assured by NHS Digital, and would like to understand the process.

### Assessment
The key point with this scenario (from an NHS Digital perspective) is that the supplier currently has no customer. The aim is to support the development of the product to a phase that NHS Digital can technically assure the solution. Once Acme Online have found a customer, the assurance process will be formally completed through a first of type deployment with their customer. Once completed the solution will be 'fully assured'.

### How Scenario 1 is played out
1. The developer can use this site to understand how to develop against in the SMSP API. The [getting started](smsp_getting_started.html) page will allow a developer with suitable [environment](smsp_test_environments.html) access to very quickly connect to the SMSP API and start playing using the [test data](smsp_test_data.html) provided.
2. The developed will be able to use [Test tools](smsp_test_tools.html) for local only development, and online  [environments](smsp_test_environments.html) available via N3 or Non-N3 connections.
2. Once the developer has understood the initial requirements to call the SMSP API, they will need to understand the web  service interface behaviour requirements (error handling, exceptions, vocabs), and the wider [foundation](foundations_reqs.html) and [demographics](demographics_reqs.html) functional requirements. These requirements cover such things as IG, Audit, Demographics specific.
3. The developer will work to the point that the solution has implemented.

..* the web service interface behaviours 
..* the foundation functional requirements
..* the demographics functional requirements

4a. The supplier will provide two artifacts to NHS Digital:

..* Acme Online will test the developed interface against the Toolkit Workbench (TKW) (Test tool](smsp_test_tools.html). This tool provides a suite of automated tests, which generate evidence for submission to NHS Digital.
..* At the same time Acme Online will complete a Target Operating Model for submission to NHS Digital. 

5. Assuming technical tests have passed, the next step is to connect into a Path-to-Live (PTL) environment. This step provides value to Acme Online as they will learn the endpoint registration steps and pipe-clean their network connect, important steps prior to going live.
6. Once successfully connected to the PTL environment Acme Online will be asked to performed some limited testing.
7. End of Technical Assurance.

In parallel to the technical work Acme Online will complete and submit to NHS Digital a target operating model [TOM](smsp_tom.html).

Once the TOM is accepted and technical testing is complete Acme Online will be aware an Assurance Certificate caveat that they are awaiting a First of Type. This status will be reflected via the NHS Digital online catalogue.

--- 

## Scenario 2 - New App Supplier with a customer
Acme Apps have developed in conjunction with a local care organisation a new mobile application for pre-op assessments. The pre-op form is completed by a healthcare professional along with the patient. The supplier would like th application to link into the NHS Digital demographics service. Acme Apps are aware they need to be assured by NHS Digital, and would like to understand the process.

### Assessment
This scenario involves both a supplier and customer (typically a care organisation), meaning the assurance can progress all the way to a live first of type (assuming the usage and settings is accepted by NHS Digital).

### How Scenario 2 is played out
Acme Apps in conjunction with their customer will complete and submit to NHS Digital Phase 1 of target operating model [TOM](smsp_tom.html). The information in Phase 1 provides details of the usage and settings of the proposed service, sufficient to allow the demographics programme to assess the application and approve or reject (with details).

The technical steps are exactly the same as Scenario 1. 

Once technically assured and a fully completed TOM (phase 1 and 2) has been submitted and approved, the solution will move into a live first of type deployment verification period (typically two weeks).

Successfully completion of the verification period, with no issues raises, to allow the status of the assurance against the Acme Apps product to be reflected as fully assured. 

{% include links.html %}