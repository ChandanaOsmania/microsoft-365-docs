---
title: Microsoft Defender for Endpoint on Android - Privacy information
description: Privacy controls, how to configure policy settings that impact privacy and information about the diagnostic data collected in Microsoft Defender for Endpoint on Android.
keywords: microsoft, defender, Microsoft Defender for Endpoint, android, privacy, diagnostic
ms.service: microsoft-365-security
ms.mktglfcycl: deploy
ms.sitesec: library
ms.pagetype: security
ms.author: macapara
author: mjcaparas
ms.localizationpriority: medium
manager: dansimp
audience: ITPro
ms.collection: 
- m365-security
- tier3
ms.topic: conceptual
ms.subservice: mde
search.appverid: met150
---

# Microsoft Defender for Endpoint on Android - Privacy information

**Applies to:**
- [Microsoft Defender for Endpoint Plan 1](https://go.microsoft.com/fwlink/p/?linkid=2154037)
- [Microsoft Defender for Endpoint Plan 2](https://go.microsoft.com/fwlink/p/?linkid=2154037)
- [Microsoft 365 Defender](https://go.microsoft.com/fwlink/?linkid=2118804)

> Want to experience Microsoft Defender for Endpoint? [Sign up for a free trial.](https://signup.microsoft.com/create-account/signup?products=7f379fee-c4f9-4278-b0a1-e4c8c2fcdf7e&ru=https://aka.ms/MDEp2OpenTrial?ocid=docs-wdatp-exposedapis-abovefoldlink)

Defender for Endpoint on Android collects information from your configured Android devices and stores it in the same tenant where you have Defender for Endpoint. The information is collected to help keep Defender for Endpoint for Android secure, up-to-date, performing as expected, and to support the service.

For more information about data storage, see [Microsoft Defender for Endpoint data storage and privacy](data-storage-privacy.md).

Information is collected to help keep Defender for Endpoint for Android secure, up-to-date, performing as expected and to support the service.

For more information on most common privacy questions about Microsoft Defender for Endpoint on Android and iOS mobile devices, see [Microsoft Defender for Endpoint and your privacy on Android and iOS mobile devices](https://support.microsoft.com/topic/microsoft-defender-for-endpoint-and-your-privacy-on-android-and-ios-mobile-devices-4109bc54-8ec5-4433-9c33-d359b75ac22a).

## Required Data

Required data consists of data that is necessary to make Defender for Endpoint for Android work as expected. This data is essential to the operation of the service and can include data related to the end user, organization, device, and apps. Here's a list of the types of data being collected:

### App information

Information about **malicious** Android application packages (APKs) on the device including

- Install source
- Storage location (file path) of the APK
- Time of install, size of APK and permissions

For Android Enterprise Fully managed devices - Information about Android application packages (APKs) installed on the device including

- Name and package name of the app
- Version number of the app
- Vendor name

For Android Enterprise with a work profile - Information about Android application packages (APKs) installed on the Work profile of the device including

- Name and package name of the app
- Version number of the app
- Vendor name

*Your organization can also choose to configure Defender for Endpoint to send information about all apps installed on the device. By default, this information is not sent to your organization.*


### Web page / Network information

- Full URL of the website only when a malicious connection or web page is detected and blocked.
- Connection information
- Protocol type (such as HTTP, HTTPS, etc.)

### Device and account information

- Device information such as date & time, Android version, OEM model, CPU info, and Device identifier.
- Device identifier is one of the below:
  - Wi-Fi adapter MAC address
  - [Android ID](https://developer.android.com/reference/android/provider/Settings.Secure#ANDROID_ID) (as generated by Android at the time of first boot of the device).
  - Randomly generated globally unique identifier (GUID).

- Tenant, Device and User information
  - Azure Active Directory (AD) Device ID and Azure User ID: Uniquely identifies the device, User respectively at Azure Active directory.
  - Azure tenant ID: GUID that identifies your organization within Azure Active Directory.
  - Microsoft Defender for Endpoint org ID: Unique identifier associated with the enterprise that the device belongs to. Allows Microsoft to identify whether issues are impacting a select set of enterprises and how many enterprises are impacted.
  - User Principal Name: Email ID of the user

### Product and service usage data

The following information is collected only for Microsoft Defender for Endpoint app installed on the device. 

- App package info, including name, version, and app upgrade status.
- Actions performed in the app.
- Threat detection information, such as threat name, category, etc.
- Crash report logs generated by Android.

## Optional Data

Optional data includes diagnostic data and feedback data. Optional diagnostic data is additional data that helps us make product improvements and provides enhanced information to help us detect, diagnose, and fix issues. Optional diagnostic data includes:

- App, CPU, and network usage.
- State of the device from the app perspective, including scan status, scan timings, app permissions granted, and upgrade status.
- Features configured by the admin.
- Basic information about the browsers on the device.

**Feedback Data** is collected through in-app feedback provided by the user

- The user's email address, if they choose to provide it.
- Feedback type (smile, frown, idea) and any feedback comments submitted by the user.
