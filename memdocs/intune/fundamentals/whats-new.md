---
# required metadata
title: What's new in Microsoft Intune
titleSuffix:
description: Find out what's new in Microsoft Intune
keywords:
author: brenduns
ms.author: brenduns
manager: dougeby
ms.date: 01/27/2023
ms.topic: conceptual
ms.service: microsoft-intune
ms.subservice: fundamentals
ms.localizationpriority: high
ms.assetid: 791ed23f-bd13-4ef0-a3dd-cd2d7332c5cc

# optional metadata

#ROBOTS:
#audience:

ms.reviewer: lebacon
ms.suite: ems
search.appverid: MET150
#ms.tgt_pltfrm:
ms.custom: intune-azure; get-started
ms.collection: 
  - M365-identity-device-management
  - highseo
---

# What's new in Microsoft Intune

Learn what's new each week in Microsoft Intune.

You can also read:  
- [**Important notices**](#notices)
- [Past releases](whats-new-archive.md) in the What's new archive
- Information about [how Intune service updates are released](https://techcommunity.microsoft.com/t5/Intune-Customer-Success/Microsoft-Intune-Service-Updates/ba-p/358728)

> [!NOTE]
> Each [monthly update](https://techcommunity.microsoft.com/t5/Intune-Customer-Success/Microsoft-Intune-Service-Updates/ba-p/358728) may take up to three days to rollout and will be in the following order:
>
> - Day 1: Asia Pacific (APAC)
> - Day 2: Europe, Middle East, Africa (EMEA)
> - Day 3: North America
> - Day 4+: Intune for Government
>
> Some features may roll out over several weeks and might not be available to all customers in the first week.
>
> For a list of upcoming Intune feature releases, see [In development for Microsoft Intune](../fundamentals/in-development.md). For new information about Autopilot, see [Windows Autopilot What's new](../../autopilot/windows-autopilot-whats-new.md).

You can use RSS to be notified when this page is updated. For more information, see [How to use the docs](../../use-docs.md#notifications).
<!-- **RSS feed**: Get notified when this page is updated by copying and pasting the following URL into your feed reader: `https://learn.microsoft.com/api/search/rss?search=%22What%27s+new+in+microsoft+intune%3F+-+Azure%22&locale=en-us` -->

<!-- Common categories:
### App management
### Device configuration
### Device enrollment
### Device management
### Device security
### Intune apps
### Monitor and troubleshoot
### Role-based access control
### Scripts
### Tenant administration
-->
## Week of February 6, 2023

### Tenant administration

#### Apply recommendations and insights to enrich the Configuration Manager site health and device management experience<!--16957774 -->

You can now use the Microsoft Endpoint Manager admin center to view recommendations and insights for your Configuration Manager sites. These recommendations can help you improve the site health and infrastructure and enrich the device management experience.

Recommendations include:  

- How to simplify your infrastructure
- Enhance device management
- Provide device insights
- Improve the health of the site

To view recommendations, open the [Microsoft Endpoint Manager admin center](https://go.microsoft.com/fwlink/?linkid=2109431) and go to **Tenant administration** > **Connectors and tokens** > **Microsoft Endpoint Configuration Manager**,  and select a *site* to view recommendations for that site.  Once selected, you’ll find the *Recommendations* tab that displays each insight along with a *Learn more* link that opens details on how to apply that recommendation.

## Week of January 30, 2023

### Device management

#### HTC Vive Focus 3 supported on Microsoft Intune for Android Open Source Devices<!--15670082--> 

Microsoft Intune for Android open source project devices (AOSP) now supports HTC Vive Focus 3. 

For more information go to [Operating systems and browsers supported by Microsoft Intune](../fundamentals/supported-devices-browsers.md)

Applies to:

- Microsoft Intune (AOSP)
#### Introducing support for laser pointers in Remote Help<!-- 16108312 -->

In Remote Help, you can now use a laser pointer when you are providing assistance on Windows.

For more information on Remote Help, go to [Remote Help](../remote-actions/remote-help.md).

Applies to:

 - Windows 10/11
## Week of January 23, 2023 (Service release 2301)

### App management

#### Configure whether to show Configuration Manager apps in Windows Company Portal<!-- 9135109 -->
In Intune you can choose whether to show or hide Configuration Manager apps from appearing in the Windows Company Portal. This option is available in [Microsoft Endpoint Manager admin center](https://go.microsoft.com/fwlink/?linkid=2109431) by selecting **Tenant administration** > **Customization**. Next to **Settings**, select **Edit**. The option to **Show** or **Hide** the Configuration Manager applications are located in the **App Sources** section of the pane. For related information about configuring the Company Portal app, see [How to configure the Intune Company Portal apps, Company Portal website, and Intune app](../apps/company-portal-app.md).

#### Block pinning web pages to Managed Home Screen app<!-- 15593458 -->
On Android Enterprise dedicated devices using Managed Home Screen, you can now use app configuration to configure the Managed Home Screen app to block pinning browser web pages to Managed Home Screen. The new `key` value is `block_pinning_browser_web_pages_to_MHS`. For more information, see [Configure the Microsoft Managed Home Screen app for Android Enterprise](../apps/app-configuration-managed-home-screen-app.md).

### Device management

#### Grace period status visible in Microsoft Intune app for Android<!-- 13498225 -->  
The Microsoft Intune app for Android now shows a grace period status to account for devices that don't meet compliance requirements but are still within their given grace period. Users can see the date by which devices must be compliant, and the instructions for how to become compliant. If they don't update their device by the given date, the device is marked as noncompliant. For more information, see the following docs:  
- [Configure compliance policies with actions for noncompliance](../protect/actions-for-noncompliance.md#available-actions-for-noncompliance)    
- [Check compliance status](../user-help/check-compliance-microsoft-intune-app-android.md)  


#### Software update policies for macOS are now generally available<!-- 12393100 -->   
Software update policies for macOS devices are now generally available. This general availability applies to supervised devices running macOS 12 (Monterey) and later. We will continue to add improvements to this feature going forward.  

For more information, see [Use Microsoft Intune policies to manage macOS software updates](../protect/software-updates-macos.md).

#### Windows Autopilot device diagnostics<!-- 16697347 -->
Windows Autopilot diagnostics is available to download in Microsoft Endpoint Manager admin center from either in the Autopilot deployments monitor or Device Diagnostics monitor for an individual device.

### Device enrollment

#### Enrollment notifications now generally available<!-- 16545401 -->
Enrollment notifications are now generally available, and are supported on Windows, Apple, and Android devices. This feature is only supported with user-driven enrollment methods. For more information, see [Set up enrollment notifications](../enrollment/enrollment-notifications.md).  

#### Skip or show Terms of Address pane in Setup Assistant<!-- 14661838 -->  
Configure Microsoft Intune to skip or show a new Setup Assistant pane called **Terms of Address** during Apple Automated Device Enrollment. The Terms of Address pane lets users on iOS/iPadOS and macOS devices personalize their device by selecting how the system addresses them: feminine, neutral, or masculine.  The pane is visible during enrollment by default, and is available for select languages.  You can hide it on devices running iOS/iPadOS 16 and later, and macOS 13 and later. For more information about the Setup Assistant screens supported in Intune, see:  

- [Setup Assistant screens for Macs](../enrollment/device-enrollment-program-enroll-macos.md#setup-assistant-screen-reference)
- [Setup Assistant screens for iOS/iPadOS](../enrollment/device-enrollment-program-enroll-ios.md#setup-assistant-screen-reference)

### Device security

#### Microsoft Tunnel for Mobile Application Management for iOS/iPadOS (Preview)<!-- 15769204, 9851288 -->  

As a public preview, you can use the Mobile Application Management (MAM) to the Microsoft Tunnel VPN gateway for iOS/iPadOS. With this preview for iOS devices that have not enrolled with Intune, supported apps on those unenrolled devices can use Microsoft Tunnel to connect to your organization when working with corporate data and resources. This includes VPN gateway support for:

- Secure access to on-premises apps and resources using modern authentication
- Single Sign On and conditional access

For more information, go to:

- [Microsoft Tunnel for Mobile Application Management for iOS/iPadOS admin guide (public preview)](../protect/microsoft-tunnel-mam-ios.md)
- [Microsoft Tunnel for MAM iOS SDK developer guide](../developer/tunnel-mam-ios-sdk.md)

Applies to:

- iOS/iPadOS

####  Attack surface reduction policy support for Security settings management for Microsoft Defender for Endpoint <!-- 13816760 -->  
Attack surface reduction policy is now supported by devices managed through the [MDE Security configuration](../protect/mde-security-integration.md#which-solution-should-i-use) scenario. To use this policy with devices that use Microsoft Defender for Endpoint but aren't enrolled with Intune:

1. In the Endpoint Security node, create a new *Attack surface reduction* policy.
2. Select **Windows 10, Windows 11, and Windows Server** as the *Platform*.
3. Select **Attack Surface Reduction Rules** for the *Profile*.  

Applies to:  
- Windows 10
- Windows 11

#### SentinelOne – New mobile threat defense partner<!-- 13911932 -->
You can now use [SentinelOne](../protect/sentinelone-mobile-threat-defense-connector.md) as an integrated Mobile Threat Defense (MTD) partner with Intune. By configuring the SentinelOne connector in Intune, you can control mobile device access to corporate resources using conditional access that's based on risk assessment in your compliance policy. The SentinelOne connector can also send risk levels to app protection policies.

### Device configuration

#### Device Firmware Configuration Interface (DFCI) will support Fujitsu devices<!--10249866 -->

For Windows 10/11 devices, you can create a DFCI profile to manage UEFI (BIOS) settings (**Devices** > **Configuration profiles** > **Create profile** > **Windows 10 and later** for platform > **Templates** > **Device Firmware Configuration Interface** for profile type).

Some Fujitsu devices running Windows 10/11 are enabled for DFCI. Contact your device vendor or device manufacturer for eligible devices.

For more information about DFCI profiles, go to:

- [Configure Device Firmware Configuration Interface (DFCI) profiles on Windows devices in Microsoft Intune](../configuration/device-firmware-configuration-interface-windows.md)
- [Device Firmware Configuration Interface (DFCI) management with Windows Autopilot](../../autopilot/dfci-management.md)

Applies to:

- Windows 10
- Windows 11

#### Support for Bulk Device Actions on devices running Android AOSP<!--15397458 -->
You can now complete "Bulk Device Actions" for devices running Android AOSP. The bulk device actions supported on devices running AOSP are Delete, Wipe and Restart.

Applies to:  
- AOSP

#### Updated descriptions for iOS/iPadOS and macOS settings in the settings catalog<!-- 16360170 -->
The settings catalog lists all the settings you can configure, and all in one place. For the iOS/iPadOS and macOS settings, for each setting category, the descriptions are updated to include more detailed information.

For more information on the settings catalog, go to:
- [Use the settings catalog to configure settings on Windows, iOS/iPadOS and macOS devices](../configuration/settings-catalog.md)
- [Common tasks you can complete using the Settings Catalog in Intune](../configuration/settings-catalog-common-features.md)

Applies to:
- iOS/iPadOS
- macOS

#### New settings available in the Apple Settings Catalog<!--16237513  -->
The [Settings Catalog](../configuration/settings-catalog.md) lists all the settings you can configure in a device policy, and all in one place.

New settings are available in the Settings Catalog. In the [Microsoft Endpoint Manager admin center](https://go.microsoft.com/fwlink/?linkid=2109431), you can see these settings at **Devices** > **Configuration profiles** > **Create profile** > **iOS/iPadOS** or **macOS** for platform > **Settings catalog** for profile type.

New settings include:

**Accounts > Subscribed Calendars**:
- Account Description
- Account Host Name
- Account Password
- Account Use SSL
- Account Username

Applies to:
- iOS/iPadOS

**Networking > Domains**:
- Cross Site Tracking Prevention Relaxed Domains

Applies to:
- macOS

The following settings are also in Settings Catalog. Previously, they were only available in Templates:

**File Vault**:
- User Enters Missing Info 

Applies to:
- macOS

**Restrictions**:
- Rating Region

Applies to:
- iOS/iPadOS

For more information about configuring Settings Catalog profiles in Intune, see [Create a policy using settings catalog](../configuration/settings-catalog.md).


#### Filter app and policy assignments by the device's Azure AD Join type (`deviceTrustType`)<!-- 8110331 -->
When you assign an app or policy, you can filter the assignment using different device properties, such as device manufacturer, operating system SKU, and more.

A new device filter property `deviceTrustType` is available for Windows 10 and later devices. With this property, you can filter app and policy assignments depending on the Azure AD Join type, with values of "Azure AD Joined", "Hybrid Azure AD Joined", and "Azure AD registered".

For more information on filters and the device properties you can use, go to:
- [Use filters when assigning your apps, policies, and profiles in Intune](filters.md)
- [Device properties, operators, and rule editing when creating filters in Intune](filters-device-properties.md)

Applies to:

- Windows 10 and later

### Monitor and troubleshoot

#### Download mobile app diagnostics in the Microsoft Endpoint Manager admin center (public preview)<!-- 9353471 -->  
Now in public preview, access user-submitted mobile app diagnostics in the admin center, including app logs sent through Company Portal app for Android, AOSP, or Windows, with support for iOS, macOS, and Microsoft Edge for iOS coming at a later date. For more information about accessing mobile app diagnostics for Company Portal, see [Configure Company Portal](../apps/company-portal-app.md#app-logs).

#### WinGet troubleshooting using diagnostic files<!-- 16724699 -->
[WinGet](/windows/package-manager/winget/) is a command line tool that enables you to discover, install, upgrade, remove, and configure applications on Windows 10 and Windows 11 devices. When working with [Win32 app management in Intune](../apps/apps-win32-app-management.md), you can now use the following file locations to help troubleshoot WinGet:
- *%TEMP%\winget\defaultstate\*.log*
- *Microsoft-Windows-AppXDeployment/Operational*
- *Microsoft-Windows-AppXDeploymentServer/Operational*

#### Intune troubleshooting pane update<!-- 4442647 -->  
A new experience for the Intune Troubleshooting pane will provide details about user's devices, policies, applications, and status. The troubleshooting pane will include the following information:

- A summary of policy, compliance, and application deployment status.
- Support for exporting, filtering, and sorting all reports.
- Support to filter by excluding policies and applications.
- Support to filter to a user’s single device.
- Details about available device diagnostics and disabled devices.
- Details about offline devices that haven't checked-in to the service for three or more days.

You can find the troubleshooting pane in [Microsoft Endpoint Manager admin center](https://go.microsoft.com/fwlink/?linkid=2109431) by selecting **Troubleshooting + support** > **Troubleshoot**. To view the new experience during preview, select **Preview upcoming changes to Troubleshooting and provide feedback** to display the **Troubleshooting preview** pane, then select **Try it now**.

#### New report for devices without compliance policy (preview)<!--14911124 --> 
We’ve added a new report named **Devices without compliance policy** to the Device compliance reports you can access through the *Reports* node of the Microsoft Endpoint Manager admin center.  This report, which is in preview, uses a  newer reporting format that provides for more capabilities.

To learn about this new organizational report, see [Devices without compliance policy (preview) (Organizational)](../fundamentals/reports.md#devices-without-compliance-policy-preview-organizational).

An older version of this report remains available through the *Devices > Monitor* page of the admin center. Eventually, that older report version will be retired, though it remains available for now.  

#### Service health messages for tenant issues that require administrative attention<!-- 14791676 -->  
The *Service health and message center page* in the Microsoft Endpoint Manager admin center can now display messages for **Issues in your environment that require action**. These messages are important communications that are sent to a tenant to alert administrators about issues in their environment that might require action to resolve. 

You can view messages for *Issues in your environment that require action* in the [Microsoft Endpoint Manager admin center](https://go.microsoft.com/fwlink/?linkid=2109431) by going to **Tenant administration** > **Tenant status** and then selecting the **Service health and message center** tab.

For more information about this page of the admin center, see [View details about your Tenant on the Intune tenant status page](../fundamentals/tenant-status.md).

### Tenant administration

#### Improved UI experience for multiple certificate connectors<!-- 16263248 -->
We’ve added pagination controls to the *Certificate connectors* view to help improve the experience when you have more than 25 certificate connectors configured. With the new controls, you can see the total number of connector records and easily navigate to a specific page when viewing your certificate connectors.

To view certificate connectors, in the [Microsoft Endpoint Manager admin center](https://go.microsoft.com/fwlink/?linkid=2109431), go to **Tenant administration** > **Connectors and tokens** > **Certificate connectors**.

### Intune apps

#### Newly available protected app for Intune<!-- 16620158 -->
The following protected app is now available for Microsoft Intune:
- Voltage SecureMail by Voltage Security

For more information about protected apps, see [Microsoft Intune protected apps](../apps/apps-supported-intune-apps.md).

### Scripts

#### Preview PowerShell script package content in Endpoint Analytics<!-- 12930245 -->
Admins can now see a preview of a PowerShell script's content for proactive remediations. The content will be displayed in a grayed-out box with scrolling capability. Admins will not be able to edit the content of the script in the preview. In [Microsoft Endpoint Manager admin center](https://go.microsoft.com/fwlink/?linkid=2109431), select **Reports** > **Endpoint analytics** > **Proactive remediations**. For related information, see [PowerShell scripts for Proactive remediations](../../analytics/powershell-scripts.md).

## Week of January 16, 2023

### App management

#### Win32 app supersedence GA<!-- 9318154 -->
We are in the process of rolling out the feature set for Win32 app supersedence GA, which will add support for apps with supersedence during ESP and also allow supersedence and dependency relationships to be added in the same app subgraph. For more information, see [Win32 app supersedence improvements](https://aka.ms/Intune/Win32-Supersedence). For information about Win32 app supersedence, see [Add Win32 app supersedence](../apps/apps-win32-supersedence.md).

## Week of January 9, 2023

### Device configuration

#### The Company Portal app enforces Password Complexity setting on Android Enterprise 12+ personally owned devices with a work profile<!-- 16211313  -->  

On Android Enterprise 12+ personally owned devices with a work profile, you can create a compliance policy and/or device configuration profile that sets the password complexity. Starting with the 2211 release, this setting is available in the Endpoint Manager admin center:

- **Devices** > **Configuration profiles** > **Create profile** > **Android Enterprise** for platform > Personally owned with a work profile
- **Devices** > **Compliance policies** > **Create policy** > **Android Enterprise** for platform > Personally owned with a work profile

The Company Portal app enforces the **Password complexity** setting.

For more information on this setting and the other settings you can configure on personally owned devices with a work profile, go to:

- [Device compliance settings for Android Enterprise in Intune](../protect/compliance-policy-create-android-for-work.md#personally-owned-work-profile)
- [Device restriction settings list for Android Enterprise in Intune](../configuration/device-restrictions-android-enterprise-personal.md)

Applies to:

- Android Enterprise 12+ personally owned devices with a work profile

## Week of December 19, 2022

### Intune apps

#### Newly available protected app for Intune<!-- 15448654 -->
The following protected app is now available for Microsoft Intune:
- Appian for Intune by Appian Corporation (Android)

For more information about protected apps, see [Microsoft Intune protected apps](../apps/apps-supported-intune-apps.md).

## Week of December 12, 2022 (Service release 2212)

### Device configuration

#### Remote Help client app includes a new option to disable chat functionality in the Tenant level setting<!-- 14685052 -->  
In the Remote Help app, admins have the option to disable chat functionality from the new tenant level setting. Turning on the disable chat feature will remove the chat button in the Remote Help app. This setting can be found in the Remote Help **Settings** tab under **Tenant Administration** in Microsoft Intune.

For more information, see [Configure Remote Help for your tenant](../remote-actions/remote-help.md#configure-remote-help-for-your-tenant).

**Applies to**: Windows 10/11

#### New settings available in the macOS Settings Catalog<!-- 16069006 -->  
The [Settings Catalog](../configuration/settings-catalog.md) lists all the settings you can configure in a device policy, and all in one place.

New settings are available in the Settings Catalog. In the [Microsoft Endpoint Manager admin center](https://go.microsoft.com/fwlink/?linkid=2109431), you can see these settings at **Devices** > **Configuration profiles** > **Create profile** > **macOS** for platform > **Settings catalog** for profile type.

New settings include:

**File Vault > File Vault Options**:

- Block FV From Being Disabled
- Block FV From Being Enabled

**Restrictions**:

- Allow Bluetooth Modification

Applies to:

- macOS

For more information about configuring Settings Catalog profiles in Intune, see [Create a policy using settings catalog](../configuration/settings-catalog.md).

#### There are default settings for SSO extension requests on iOS, iPadOS, and macOS devices<!-- 15082414-15084030 -->  

When you create a single sign-on app extension configuration profile, there are some settings you configure. The following settings will use the following default values for all SSO extension requests:

- **AppPrefixAllowList** key
  - macOS default value: `com.microsoft.,com.apple.`
  - iOS/iPadOS default value: `com.apple.`

- **browser_sso_interaction_enabled** key
  - macOS default value: `1`
  - iOS/iPadOS default value: `1`

- **disable_explicit_app_prompt** key
  - macOS default value: `1`
  - iOS/iPadOS default value: `1`

If you configure a value other than the default value, then the configured value will overwrite the default value. 

For example, you don't configure the `AppPrefixAllowList` key. By default, all Microsoft apps (`com.microsoft.`) and all Apple apps (`com.apple.`) will be enabled for SSO on macOS devices. You can overwrite this behavior by adding a different prefix to the list, such as `com.contoso.`.

For more information on the Enterprise SSO plug-in, go to [Use the Microsoft Enterprise SSO plug-in on iOS/iPadOS and macOS devices in Microsoft Intune](../configuration/use-enterprise-sso-plug-in-ios-ipados-macos.md)

Applies to:

- iOS/iPadOS
- macOS

### Device enrollment

#### Enrollment token lifetime increases to 65 years for Android Enterprise dedicated devices<!-- 15094454  -->  
Now you can create an enrollment profile for Android Enterprise dedicated devices that's valid for up to 65 years.  If you have an existing profile, the enrollment token will still expire at whatever date you chose when you created the profile, but during renewal you can extend the lifetime. For more information about creating an enrollment profile, see [Set up Intune enrollment for Android Enterprise dedicated devices](../enrollment/android-kiosk-enroll.md#create-an-enrollment-profile).

### Device management

#### Update policies for macOS now available for all supervised devices<!-- 16141990  -->  
Software update policies for macOS devices now apply to all macOS supervised devices. Previously, only those devices that enrolled through Automated Device Enrollment (ADE) would qualify to receive updates. For more information on configuring update policies for macOS, see [Use Microsoft Intune policies to manage macOS software updates](../protect/software-updates-macos.md).

Applies to:  
- macOS

#### Policy and reports for Windows feature updates and expedited quality updates are now Generally Available<!-- 15738456 -->  
Both the policies and reports for managing feature updates and quality updates (expedited updates) for Windows 10 and later, are out of preview and now generally available.

For more information about these policies and reports, see:

- [Feature updates policy](../protect/windows-10-feature-updates.md)
- [Expedite quality updates policy](../protect/windows-10-expedite-updates.md)
- [Windows Update compliance reports](../protect/windows-update-compliance-reports.md)

Applies to:  
-  Windows 10/11

## Week of November 28, 2022

### App management

#### Microsoft Store apps in Intune<!-- 12708346 -->  
You can now search, browse, configure, and deploy Microsoft Store apps within Intune. The new Microsoft Store app type is implemented using the Windows Package Manager. This app type features an expanded catalog of apps, which includes both UWP apps and Win32 apps. Roll out of this feature is expected to complete by December 2, 2022.  For more information, see [Add Microsoft Store apps to Microsoft Intune](../apps/store-apps-microsoft.md).

### Tenant administration

#### Access policies for multiple Administrator Approval (public preview)<!-- 9348867  -->
In public preview, you can use Intune *access policies* to require that a second Administrator Approval account be used to approve a change before the change is applied. This capability is known as multiple Administrator Approval (MAA).

You create an access policy to protect a type of resource, like App deployments. Each access policy also includes a group of users who are *approvers* for the changes protected by the policy. When a resource like an app deployment configuration is protected by an access policy, any changes that are made to the deployment, including creating, deleting, or modifying an existing deployment won't apply until a member of the approvers group for that access policy reviews and approves that change.

Approvers can also reject requests, and both the individual requesting a change and the approver can provide notes about the change, or why it was approved or rejected.

Access policies are supported for the following resources:

- **Apps** – Applies to [app deployments](../apps/apps-add.md), but doesn't apply to app protection policies.
- **Scripts** – Applies to deploying scripts to devices that run [macOS](../apps/macos-shell-scripts.md) or [Windows](../apps/intune-management-extension.md).

For more information, see [Use Access policies to require multiple administrative approval](../fundamentals/multi-admin-approval.md).  

### Device security

#### Microsoft Tunnel for Mobile Application Management for Android (Preview)<!-- 15769204 -->  
As a public preview, you can now use Microsoft Tunnel with unenrolled devices. This capability is called [Microsoft Tunnel for Mobile Application Management](../protect/microsoft-tunnel-mam.md) (MAM). This preview supports Android, and without any changes to your existing Tunnel infrastructure, supports the Tunnel VPN gateway for:

- Secure access to on-premises apps and resources using modern authentication
- Single Sign On and conditional access

To use Tunnel MAM, unenrolled devices must install Microsoft Edge, Microsoft Defender for Endpoint, and the Company Portal. You can then use the Microsoft Endpoint Manager admin center to configure the following profiles for the unenrolled devices:

- An App configuration profile for managed apps, to configure Microsoft Defender on devices for use as the Tunnel client app.
- A second App configuration profile for managed apps, to configure Microsoft Edge to connect to Tunnel.
- An App protection profile to enable automatic start of the Microsoft Tunnel connection.

Applies to:  
- Android Enterprise

## Week of November 14, 2022 (Service release 2211)

### App management

#### Control the display of Managed Google Play apps<!-- 621615   -->  
You can group Managed Google Play apps into collections and control the order that collections are displayed when selecting apps in Intune. You can also make apps visible via search only. This capability is available in [Microsoft Endpoint Manager admin center](https://go.microsoft.com/fwlink/?linkid=2109431) by selecting **Apps** > **All apps** > **Add** > **Managed Google Play app**. For related information, see [Add a Managed Google Play store app directly in the Intune console](../apps/apps-add-android-for-work.md#add-a-managed-google-play-store-app-directly-in-the-microsoft-endpoint-manager-admin-center).

### Device configuration

#### New password complexity setting for Android Enterprise 12+ personally owned devices with a work profile<!-- 12436068  -->  
On Android Enterprise 11 and older personally owned devices with a work profile, you can set the following password settings:

- **Compliance policies** > **Android Enterprise for platform** > **Personally owned work profile** > **System security** > **Required password type**, **Minimum password length**
- **Device configuration profiles** > **Android Enterprise for platform** > **Personally owned work profile** > **Device restrictions** > **Work profile settings** > **Required password type**, **Minimum password length**
- **Device configuration profiles** > **Android Enterprise for platform** > **Personally owned work profile** > **Device restrictions** > **Password** > **Required password type**, **Minimum password length**

Google is deprecating the **Required password type** and **Minimum password length** settings for Android 12+ personally owned devices with a work profile and replacing them with new password complexity requirements. For more information about this change, go to [Day zero support for Android 13](https://aka.ms/Intune/Android13).

The new **Password complexity** setting has the following options:

- **None**: Intune doesn't change or update this setting. By default, the OS may not require a password.
- **Low**: Pattern or PIN with repeating (4444) or ordered (1234, 4321, 2468) sequences are blocked.
- **Medium**: PIN with repeating (4444) or ordered (1234, 4321, 2468) sequences are blocked. The length, alphabetic length, or alphanumeric length must be at least 4 characters.
- **High**: PIN with repeating (4444) or ordered (1234, 4321, 2468) sequences are blocked. The length must be at least 8 characters. The alphabetic or alphanumeric length must be at least 6 characters.

On Android 12+, if you currently use the **Required password type** and **Minimum password length** settings in a compliance policy or device configuration profile, then we recommend using the new **Password complexity** setting instead.

If you continue to use the **Required password type** and **Minimum password length** settings, and don't configure the **Password complexity** setting, then new devices running Android 12+ might default to the **High** password complexity.

For more information on these settings and what happens to existing devices with the deprecated settings configured, go to:

- [Android Enterprise personally owned devices with a work profile - configuration profile settings list](../configuration/device-restrictions-android-enterprise-personal.md)
- [Android Enterprise personally owned devices with a work profile - compliance policy settings list](../protect/compliance-policy-create-android-for-work.md#personally-owned-work-profile)

Applies to:

- Android Enterprise 12.0 and newer personally owned devices with a work profile

#### New settings available in the iOS/iPadOS and macOS Settings Catalog<!-- 16068756 -->  
The [Settings Catalog](../configuration/settings-catalog.md) lists all the settings you can configure in a device policy, and all in one place.

New settings are available in the Settings Catalog. In the [Microsoft Endpoint Manager admin center](https://go.microsoft.com/fwlink/?linkid=2109431), you can see these settings at **Devices** > **Configuration profiles** > **Create profile** > **iOS/iPadOS** or **macOS** for platform > **Settings catalog** for profile type.

New settings include:

**Networking > DNS Settings**:

- DNS Protocol
- Server Addresses
- Server Name
- Server URL
- Supplemental Match Domains
- On Demand Rules
- Action
- Action Parameters
- DNS Domain Match
- DNS Server Address Match
- Interface Type Match
- SSID Match
- URL String Probe
- Prohibit Disablement

**File Vault**:

- Defer
- Defer Don't Ask At User Logout
- Defer Force At User Login Max Bypass Attempts
- Enable
- Show Recovery Key
- Use Recovery Key

**File Vault > File Vault Recovery Key Escrow**:

- Device Key
- Location

**Restrictions**:

- Allow Air Play Incoming Requests

Applies to:

- macOS

**Web > Web Content Filter**:

- Allow List Bookmarks
- Auto Filter Enabled
- Deny List URLs
- Filter Browsers
- Filter Data Provider Bundle Identifier
- Filter Data Provider Designated Requirement
- Filter Grade
- Filter Packet Provider Bundle Identifier
- Filter Packet Provider Designated Requirement
- Filter Packets
- Filter Sockets
- Filter Type
- Organization
- Password
- Permitted URLs
- Plugin Bundle ID
- Server Address
- User Defined Name
- User Name
- Vendor Config

Applies to:

- iOS/iPadOS
- macOS

For more information about configuring Settings Catalog profiles in Intune, see [Create a policy using settings catalog](../configuration/settings-catalog.md).

#### Device Firmware Configuration Interface (DFCI) will support Panasonic devices<!-- 15729353 -->  
For Windows 10/11 devices, you can create a DFCI profile to manage UEFI (BIOS) settings (**Devices** > **Configuration profiles** > **Create profile** > **Windows 10 and later** for platform > **Templates** > **Device Firmware Configuration Interface** for profile type).

New Panasonic devices running Windows 10/11 will be enabled for DFCI starting Fall 2022. So, admins can create DFCI profiles to manage the BIOS and then deploy the profiles to these Panasonic devices.

Contact your device vendor or device manufacturer to ensure you get eligible devices.

For more information about DFCI profiles, go to:

- [Configure Device Firmware Configuration Interface (DFCI) profiles on Windows devices in Microsoft Intune](../configuration/device-firmware-configuration-interface-windows.md)
- [Device Firmware Configuration Interface (DFCI) management with Windows Autopilot](/mem/autopilot/dfci-management)

Applies to:

- Windows 10
- Windows 11

#### Login and background item management support on macOS devices using the settings catalog<!-- 15751007  -->  
On macOS devices, you can create a policy that automatically opens items when users sign in to their macOS devices. For example, you can open apps, documents, and folders.

In Intune, the settings catalog includes new Service Management settings at **Devices** > **Configuration profiles** > **Create profile** > **macOS** for platform > **Settings catalog** > **Login** > **Service Management**. These settings can prevent users from disabling the managed login and background items on their devices.

For more information on the settings catalog, go to:

- [Use the settings catalog to configure settings](../configuration/settings-catalog.md)
- [Common tasks you can complete using the Settings Catalog](../configuration/settings-catalog-common-features.md)

Applies to:

- macOS 13 and newer

### Intune apps

#### Newly available protected apps for Intune<!-- 16118715, 16118848, 16135107, 16027039, 15658466, 15658598  -->  
The following protected apps are now available for Microsoft Intune:

- Varicent by Varicent US OpCo Corporation
- myBLDNG by Bldng.ai
- Enterprise Files for Intune by Stratospherix Ltd
- ArcGIS Indoors for Intune by ESRI
- Meetings by Decisions by Decisions AS
- Idenprotect Go by Apply Mobile Ltd

For more information about protected apps, see [Microsoft Intune protected apps](../apps/apps-supported-intune-apps.md).

### Monitor and troubleshoot

#### Review Cloud PC connectivity health checks and errors in Microsoft Endpoint Manager admin center<!-- 13811774 -->  
You can now review connectivity health checks and errors in the Microsoft Endpoint Manager admin center to help you understand if your users are experiencing connectivity issues. You’ll also get a troubleshooting tool to help resolve connectivity issues. To see the checks, select **Devices** > **Windows 365** > **Azure network connections** > *select a connection in the list* > **Overview**.  

### Tenant administration

#### Deliver organizational messages for Windows 11 (public preview)<!-- 15314747  -->  
Use Microsoft Intune to deliver important messages and call-to-actions to employees on their devices.  Organizational messages are preconfigured messages intended to improve employee communication in remote and hybrid-work scenarios. They can be used to help employees adapt to new roles, learn more about their organization, and stay informed of new updates and trainings. You can deliver messages  just above the taskbar, in the notifications area, or in the Get Started app on Windows 11 devices.

During public preview, you can:

* Select from a variety of preconfigured, common messages to assign to Azure AD user groups.
* Add your organization's logo. 
* Include a custom destination URL in the message that redirects device users to a specific place.
* Preview messages in 15 supported languages, in dark and light theme.
* Schedule a delivery window and message frequency.
* Track the status of messages and the number of views and clicks they receive. Views and clicks are aggregated by messages.
* Cancel scheduled or active messages.  
* Configure a new built-in role in Intune called *Organizational Messages Manager*, which allows assigned admins to view and configure messages.  

All configurations need to be done in the Microsoft Endpoint Manager admin center. The Microsoft Graph API isn't available to use with organizational messages. For more information, see [Overview of organizational messages](../remote-actions/organizational-messages-overview.md).

## Week of November 7, 2022

### App management

#### Ending support for Windows Information Protection<!-- 15991481 -->
Windows Information Protection (WIP) policies without enrollment is being deprecated. You can no longer create new WIP policies without enrollment. Until December of 2022, you will continue to be able to modify existing policies until the deprecation of the *without enrollment* scenario is complete. For related information, go to [Plan for Change: Ending support for Windows Information Protection](../fundamentals/whats-new.md#plan-for-change-ending-support-for-windows-information-protection).

### Device Configuration

#### User configuration support for Windows 11 multi-session VMs is now generally available

You can now:
 - Configure user scope policies using **Settings catalog** and assign to groups of users, including ADMX-ingested policies
 - Configure user certificates and assign to users
 - Configure PowerShell scripts to install in the user context and assign to users

Applies to:
 - **Windows 11**
 - **Virtual machines** created in [Azure Public and Azure Government clouds](/enterprise-mobility-security/solutions/ems-intune-govt-service-description)
## Week of October 31, 2022

### App management

#### Primary MTD service app protection policy setting for Intune<!-- 13222514 -->
Intune now supports both Microsoft Defender for Endpoint and one non-Mobile Threat Defense (MTD) connector to be turned “On” for App Protection Policy evaluation per platform. This enables scenarios where a customer may want to migrate between Microsoft Defender for Endpoint and non-Microsoft MTD service without a pause in protection via risk scores in App Protection Policy. A new setting has been introduced under Conditional Launch health checks titled “Primary MTD service” to specify which service should be enforced for the end user. For more information, see [Android app protection policy settings](../apps/app-protection-policy-settings-android.md) and [iOS app protection policy settings](../apps/app-protection-policy-settings-ios.md).

## Week of October 24, 2022 (Service release 2210)

### App management

#### Use filters with app configuration policies for managed devices<!-- 7423842  -->  
You can use filters to refine the assignment scope when deploying app configuration policies for managed devices. You must first [create a filter](../fundamentals/filters.md#create-a-filter) using any of the available properties for iOS and Android. Then, in [Microsoft Endpoint Manager admin center](https://go.microsoft.com/fwlink/?linkid=2109431) you can assign your managed app configuration policy by selecting **Apps** > **App configuration policies** > **Add** > **Managed devices** and go to the assignment page. After selecting a group, you can refine the applicability of the policy by choosing a filter and deciding to use it in **Include** or **Exclude** mode. For related information about filters, see [Use filters when assigning your apps, policies, and profiles in Microsoft Endpoint Manager admin center](../fundamentals/filters.md).

### Device configuration

#### Group Policy analytics automatically applies scope tags assigned to admins when they import Group Policy objects<!-- 16017499 -->  
In Group Policy analytics, you can import your on-premises GPOs to see the policy settings that support cloud-based MDM providers, including Microsoft Intune. You can also see any deprecated settings or settings not available.

Now, scope tags assigned to admins are automatically applied when these admins import GPOs into Group Policy analytics.

For example, admins have "Charlotte", "London", or "Boston" scope tags assigned to their role:

- An admin with the "Charlotte" scope tag imports a GPO. 
- The "Charlotte" scope tag is automatically applied to the imported GPO.
- All admins with the "Charlotte" scope tag can see the imported object.
- Admins with only the "London" or only the "Boston" scope tags can't see the imported object from the "Charlotte" admin.

For admins to see the analytics or migrate the imported GPO to an Intune policy, these admins must have one of the same scope tags as the admin that did the import.

For more information on these features, go to:

- [Analyze your on-premises GPOs using Group Policy analytics in Microsoft Intune](../configuration/group-policy-analytics.md)
- [Use role-based access control (RBAC) and scope tags for distributed IT](scope-tags.md)

Applies to:

- Windows 11
- Windows 10

#### New network endpoints for Microsoft Intune<!--15847055 -->

New network endpoints have been added to our documentation to accommodate new Azure Scale Units (ASU) that have been added to the Intune service. We recommend updating your firewall rules with the latest list of IP addresses to ensure that all network endpoints for Microsoft Intune are up-to-date.

For the full list go to  [Network endpoints for Microsoft Intune](intune-endpoints.md).

#### Filter app and group policy assignments using Windows 11 SE operating system SKUs<!-- 10588651  -->  
When you assign an app or policy, you can filter the assignment using different device properties, such as device manufacturer, operating system SKU, and more.

Two new Windows 11 SE operating system SKU's are available. You can use these SKUs in your assignment filters to include or exclude Windows 11 SE devices from applying group-targeted policies and applications. 

For more information on filters and the device properties you can use, go to:

- [Use filters when assigning your apps, policies, and profiles in Microsoft Endpoint Manager](filters.md)
- [Device properties, operators, and rule editing when creating filters in Microsoft Endpoint Manager](filters-device-properties.md)

Applies to:

- Windows 11 SE

#### New settings available in the iOS/iPadOS and macOS settings catalog <!-- 15514929  -->  
The [settings catalog](../configuration/settings-catalog.md) lists all the settings you can configure in a device policy, and all in one place.

New settings are available in the settings catalog. In the [Microsoft Endpoint Manager admin center](https://go.microsoft.com/fwlink/?linkid=2109431), you can see these settings at **Devices** > **Configuration profiles** > **Create profile** > **iOS/iPadOS** or **macOS** for platform > **Settings catalog** for profile type.

New settings include:

**Networking > Cellular**:

- Enable XLAT464

Applies to:

- iOS/iPadOS

**Privacy > Privacy Preferences Policy Control**:

- System Policy App Bundles

Applies to:

- macOS

**Restrictions**:

- Allow Rapid Security Response Installation
- Allow Rapid Security Response Removal

Applies to:

- iOS/iPadOS
- macOS

For more information about configuring settings catalog profiles in Intune, see [Create a policy using settings catalog](../configuration/settings-catalog.md).

#### New settings for Device Firmware Configuration Interface (DFCI) profiles on Windows devices<!-- 15511597  -->  
You can create a DFCI profile that enables the Windows OS to pass management commands from Intune to UEFI (Unified Extensible Firmware Interface) (**Devices** > **Configuration profiles** > **Create profile** > **Windows 10 and later** for platform > **Templates > Device Firmware Configuration Interface**)

You can use this feature to control BIOS settings. There are new settings you can configure in the DFCI policy:

- Cameras:
  - Front camera
  - Infrared camera
  - Rear camera

- Radios:
  - WWAN
  - NFC

- Ports
  - SD Card

For more information on DFCI profiles, go to:

- [Use Device Firmware Configuration Interface (DFCI) profiles on Windows devices in Microsoft Intune](../configuration/device-firmware-configuration-interface-windows.md)
- [DFCI profile settings list](../configuration/device-firmware-configuration-interface-windows-settings.md)

Applies to:

- Windows 11 on supported UEFI
- Windows 10 RS5 (1809) and later on supported UEFI

### Device enrollment

#### iOS/iPadOS Setup Assistant with modern authentication supports Just in Time Registration (public preview)<!-- 15515188 -->  
Intune supports Just in Time (JIT) Registration for iOS/iPadOS enrollment scenarios that use Setup Assistant with modern authentication. JIT Registration reduces the number of authentication prompts shown to users throughout the provisioning experience, giving them a more seamless onboarding experience. It eliminates the need to have the Company Portal app for Azure AD registration and compliance checks, and establishes single sign-on across the device. JIT Registration is available in public preview for devices enrolling through Apple automated device enrollment and running iOS/iPadOS 13.0 or later. For more information, see [Authentication methods for automated device enrollment](../enrollment/automated-device-enrollment-authentication.md). 

### Device management

#### Connect Chrome OS devices in Intune (public preview)<!-- 14273312 -->  
View company or school-owned devices that run on Chrome OS in the Microsoft Endpoint Manager admin center.  Now in public preview, you can establish a connection between the Google Admin console and Microsoft Endpoint Manager admin center.  Device information about your Chrome OS endpoints is synced into Intune and viewable in your device inventory list. Basic remote actions, such as restart, wipe, and lost mode are also available in the admin center. For more information about how to set up a connection, see [Configure Chrome Enterprise connector](../enrollment/chrome-enterprise-connector-configure.md).  

#### Manage macOS software updates with Intune<!-- 9801186 -->  
You can now use Intune policies to manage macOS software updates for devices that enrolled using Automated Device Enrollment (ADE).  See [Manage macOS software update policies in Intune](../protect/software-updates-macos.md).

Intune supports the following macOS update types:

- Critical updates
- Firmware updates
- Configuration file updates
- All other updates (OS, built-in apps)

In addition to scheduling when a device updates, you can manage behaviors like the following:

- Download and install: Download or install the update, depending on the current state.
- Download only: Download the software update without installing it.
- Install immediately: Download the software update and trigger the restart countdown notification.
- Notify only:  Download the software update and notify the user through the App Store.
- Install later: Download the software update and install it at a later time.
- Not configured: No action taken on the software update.

For information from Apple about managing macOS software updates, see [Manage software updates for Apple devices - Apple Support](https://support.apple.com/guide/deployment/manage-software-updates-depc4c80847a/web) in the Apple's Platform Deployment documentation.
Apple maintains a list of security updates at [Apple security updates - Apple Support](https://support.apple.com/en-us/HT201222).

#### Deprovision Jamf Pro from within the Microsoft Endpoint Manager admin center<!-- 3485465  -->  
You can now [deprovision your Jamf Pro to Intune integration](../protect/conditional-access-jamf-cloud-connector.md#deprovision-jamf-pro-from-within-the-microsoft-endpoint-manager-admin-center) from within the Microsoft Endpoint Manager admin center. This can be useful should you no longer have access to the Jamf Pro console, through which you can also deprovision integration.

This capability functions similarly to disconnecting Jamf Pro from within the Jamf Pro console, in that after you remove the integration, your organization's Mac devices are removed from Intune after 90 days.

#### New hardware details available for individual devices running on iOS/iPadOS<!-- 15038076  -->  
Select **Devices** > **All devices** > *select one of your listed devices* and open it's **Hardware** details. The following new details are available in the **Hardware** pane of individual devices:

- **Battery level**: Shows the battery level of the device anywhere between 0 and 100, or defaults to null if the battery level cannot be determined. This is available for devices running iOS/iPadOS 5.0 and later.
- **Resident users**: Shows the number of users currently on the shared iPad device, or defaults to null if the number of users cannot be determined. This is available for devices running iOS/iPadOS 13.4 and later.

For more information, go to [View device details with Microsoft Intune](../remote-actions/device-inventory.md).

Applies to

- iOS/iPadOS

#### Use the `$null` value in filters<!-- 11030128  -->  
When you assign apps and policies to groups, you can use filters to assign a policy based on rules you create (**Tenant administration** > **Filters** > **Create**). These rules use different device properties, such as category or the enrollment profile.

Now, you can use the `$null` value with the `-Equals` and `-NotEquals` operators.

For example, use the `$null` value in the following scenarios:

- You want to target all devices that don't have a category assigned to the device.
- You want to target devices that don't have an enrollment profile property assigned to the device.

For more information on filters and the rules you can create, go to:

- [Use filters when assigning your apps, policies, and profiles in Microsoft Intune](filters.md)
- [Device properties, operators, and rule editing when creating filters in Microsoft Intune](filters-device-properties.md)

Applies to:

- Android device administrator
- Android Enterprise
- iOS/iPadOS
- macOS
- Windows 10/11

### Device security

#### Reusable groups of settings for removable storage in Device Control profiles (preview) <!-- 7351534 -->  
In public preview, you can use [reusable groups of settings](../protect/reusable-settings-groups.md) with [device control profiles](../protect/endpoint-security-asr-policy.md#add-reusable-settings-groups-to-profiles-for-device-control) in your attack surface reduction policies.

The reusable groups for device control profiles include a collection of settings that support managing *read*, *write*, and *execute* access for removable storage. Examples of common scenarios include:

- Prevent write and execute access to all but allow specific approved USBs
- Audit write and execute access to all but block specific unapproved USBs
- Only allow specific user groups to access specific removable storage on a shared PC

Applies to:  
- Windows 10 or later

#### Reusable groups of settings for Microsoft Defender Firewall Rules (preview) <!-- 5653346, 6009541 -->  
In public preview, you can use [reusable groups of settings](../protect/reusable-settings-groups.md) that you can use with [profiles for Microsoft Defender Firewall Rules](../protect/endpoint-security-firewall-policy.md#add-reusable-settings-groups-to-profiles-for-firewall-rules). The reusable groups are collections of remote IP addresses and FQDNs that you define one time and can then use with one or more firewall rule profiles. You’ll no longer need to reconfigure the same group of IP addresses in each individual profile that might require them.

Features of the reusable settings groups include:

- Add one or more remote IP addresses.

- Add one or more FQDNs that can auto resolve to the remote IP address, or for one or more simple keywords when auto resolve for the group is off.

- Use each settings group with one or more firewall rule profiles and the different  profiles can support different access configurations for the group.

  For example, you can create two firewall rule profiles that reference the same reusable settings group and assign each profile to a different group of devices. The first profile can block access to all the remote IP addresses in the reusable settings group, while the second profile can be configured to allow access.

- Edits to a settings group that's in use are automatically applied to all Firewall Rules profiles that use that group.  

#### Attack surface reduction rule exclusions on a per-rule basis<!-- 13385644   -->  
You can now [configure per-rule exclusions for Attack surface reduction rules policies](../protect/endpoint-security-asr-policy.md#exclusions-for-attack-surface-reduction-rules). Per-rule exclusions are enabled through a new per-rule setting **ASR Only Per Rule Exclusions**.

When you create or edit attack surface reduction rule policies and change a setting that supports exclusions from the default of *Not configured* to any of the other available options, the new per-setting exclusion option becomes available. Any configurations for that settings instance of *ASR Only Per Rule Exclusions* will apply to only that setting.

You can continue to configure global exclusions that apply to all attack surface reduction rules on the device
by using the setting **Attack Surface Reduction Only Exclusions**.

Applies to:

- Windows 10/11

> [!NOTE]  
> ASR polices do not support merge functionality for *ASR Only Per Rule Exclusions* and a policy conflict can result when multiple polices that configure *ASR Only Per Rule Exclusions* for the same device conflict. To avoid conflicts, combine the configurations for *ASR Only Per Rule Exclusions* into a single ASR policy. We are investigating adding policy merge for *ASR Only Per Rule Exclusions* in a future update.

#### Grant apps permission to silently use certificates on Android Enterprise devices<!-- 12441244    -->  
You can now configure silent use of certificates by apps on Android Enterprise devices that enrolled as **Fully Managed, Dedicated, and Corporate-Owned work Profile**.

This capability is available on a new **Apps** page in the certificate profile configuration workflow by setting **Certificate access** to  **Grant silently for specific apps (require user approval for other apps)**.  With this configuration, the apps you then select will silently use the certificate. All other apps continue to use the default behavior which is to require user approval.

This capability is supported for the following certificate profiles for only Android Enterprise Fully Managed, Dedicated, and Corporate-Owned work Profiles:

- [Derived credentials](../protect/derived-credentials.md#use-derived-credentials-for-app-authentication)
- [Imported PKCS](../protect/certificates-imported-pfx-configure.md#create-a-pkcs-imported-certificate-profile)
- [PKCS](../protect/certificates-pfx-configure.md#create-a-pkcs-certificate-profile)
- [SCEP](../protect/certificates-profile-scep.md#create-a-scep-certificate-profile)

#### In-app notifications for Microsoft Intune app<!-- 13110609  -->  
Android Open Source Project(AOSP) device users can now receive compliance notifications in the Microsoft Intune app. This capability is only available on AOSP user-based devices. For more information, see [AOSP compliance notifications](../user-help/check-compliance-aosp.md#compliance-notifications).

### Intune apps

#### Newly available protected apps for Intune<!-- 15287512, 15448552   -->  
The following protected apps are now available for Microsoft Intune:

- MyITOps for Intune by MyITOps, Ltd
- MURAL - Visual Collaboration by Tactivos, Inc

For more information about protected apps, see [Microsoft Intune protected apps](../apps/apps-supported-intune-apps.md).

## Week of October 17, 2022

### App management

#### Enhanced app picker for managed apps on Android devices<!-- 14531483 -->

Android device users can select, view, and remove their default app selections in the Intune Company Portal app. Company Portal securely stores the device user's default choices for managed apps. Users can view and remove their selections in the Company Portal app by going to **Settings** > **Default Apps** > **See defaults**. This feature is an enhancement to the Android custom app picker for managed apps, which is a part of the Android MAM SDK. For more information about how to view default apps, see [View and edit default apps](../user-help/use-managed-apps-on-your-device-android.md#view-and-edit-default-apps). 

## Week of October 10, 2022

### Device management

#### Microsoft Endpoint Manager branding change<!-- 15812021 -->  
As of October 12, 2022, the name Microsoft Endpoint Manager will no longer be used. Going forward, we’ll refer to cloud-based unified endpoint management as Microsoft Intune and on-premises management as Microsoft Configuration Manager. With the launch of advanced management, Microsoft Intune will also become the name of our growing product family for endpoint management solutions at Microsoft.  For details, see [the official announcement](https://aka.ms/itsintune) on the endpoint management Tech Community blog. Documentation changes are ongoing to remove Microsoft Endpoint Manager.

For related information, see [Endpoint management documentation]( ../../index.yml).

#### Grace period status visible in Windows Company Portal<!-- 14746606 -->  
Windows Company Portal now displays a grace period status to account for devices that don't meet compliance requirements but are still within their given grace period. Users are shown the date by which they need to become compliant and the instructions for how to become compliant. If users don't update their device by the given date, their device status changes to noncompliant. For more information about setting grace periods, see [Configure compliance policies with actions for noncompliance](../protect/actions-for-noncompliance.md#available-actions-for-noncompliance) and [Check access from Device details page](../user-help/check-device-access-windows-cpapp.md#check-access-from-device-details-page).

#### Linux device management available in Microsoft Intune<!-- 14616038 -->  
Microsoft Intune now supports Linux device management for devices running Ubuntu Desktop 22.04 or 20.04 LTS. Intune admins don't need to do anything to enable Linux enrollment in the Microsoft Endpoint Manager admin center.  Linux users can [enroll supported Linux devices](../user-help/enroll-device-linux.md) on their own and use the Microsoft Edge browser to access corporate resources online.

In the admin center, you can:

- Enforce Conditional Access policies in Microsoft Edge.  
- [Create a Linux device compliance policy](../protect/device-compliance-get-started.md#device-compliance-policies) with rules about:  
  - Allowed distributions
  - Custom compliance
  - Device encryption
  - Password policy
- [Apply custom compliance settings](../protect/compliance-use-custom-settings.md) using POSIX-compliant shell scripts for discovery, and JSON files to define the custom settings you want to use.

## Week of October 03, 2022

### Device Security

#### Non-compliance warning message includes a link<!--13694184  -->  
In Remote Help, a link has been added to the non-compliance warning notification **View device compliance information** and it allows a helper to learn more about why the device is not compliant in Microsoft Endpoint Manager.

For more information, go to:

- [Microsoft Intune Remote Help](../remote-actions/remote-help.md)

- [Monitor Device compliance](../protect/compliance-policy-monitor.md)

Applies to:
**Windows 10/11**

## Week of September 26, 2022

### Monitor and troubleshoot

#### Open Help and Support without losing your context in the Microsoft Endpoint Manager admin center<!-- 12469338 -->  
You can now use the **?** icon in the Microsoft Endpoint Manager admin center to open a [help and support](../../get-support.md) session without losing your current node of focus in the admin center. The **?** icon is always available in the upper right of the title bar of the admin center. This change adds an additional method for accessing *Help and support*.

When you select **?**, the admin center opens the help and support view in a new and separate side-by-side pane. By opening this separate pane, you’ll be free to navigate the support experience without affecting your original location and focus on the admin center.

## Week of September 19, 2022 (Service release 2209)

### App management

#### New app types for Microsoft Endpoint Manager<!-- 7210233 -->
As an admin, you will be able to create and assign two new types of Intune apps:
- **iOS/iPadOS web clip** 
- **Windows web link**

These new app types work in a similar way to the existing **web link** application type, however they apply only for their specific platform, whereas web link applications apply across all platforms. With these new app types, you can assign to groups and also use assignment filters to limit the scope of assignment. You will find this functionality in [Microsoft Endpoint Manager admin center](https://go.microsoft.com/fwlink/?linkid=2109431), by selecting **Apps** > **All Apps** > **Add**.

### Device management

#### Microsoft Intune will be ending support for Windows 8.1<!-- 14740233 -->
Microsoft Intune will be ending support on October 21, 2022 for devices running Windows 8.1. After that date, technical assistance and automatic updates that help protect your devices running Windows 8.1 will no longer be available. Additionally, because the sideloading scenario for line-of-business apps is only applicable to Windows 8.1 devices, Intune will no longer support Windows 8.1 sideloading. Sideloading is installing, and then running or testing an app that isn't certified by the Microsoft Store. In Windows 10/11, "sideloading" is simply setting a device config policy to include "Trusted app installation". For more information, see [Plan for Change: Ending support for Windows 8.1](../fundamentals/whats-new.md#plan-for-change-ending-support-for-windows-81-).

#### Group member count visible in assignments<!-- 13434676 -->
When assigning policies in the admin center, you can now see the number of users and devices in a group. Having both counts will help you pinpoint the right group and understand the impact the assignment has before you apply it.

### Device configuration

#### New lock screen message when adding custom support information to Android Enterprise devices<!-- 13158348 -->
On Android Enterprise devices, you can create a device restrictions configuration profile that shows a custom support message on the devices (**Devices** > **Configuration profiles** > **Create profile** > **Android Enterprise** > **Fully managed, dedicated, and corporate-owned work profile** for platform > **Device restrictions** for profile type > **Custom support information**).

There's a new setting you can configure:
- **Lock screen message**: Add a message that's shown on the device lock screen. 

When you configure the **Lock screen message**, you can also use the following device tokens to show device-specific information:
- `{{AADDeviceId}}`: Azure AD device ID
- `{{AccountId}}`: Intune tenant ID or account ID
- `{{DeviceId}}`: Intune device ID
- `{{DeviceName}}`: Intune device name
- `{{domain}}`: Domain name
- `{{EASID}}`: Exchange Active Sync ID
- `{{IMEI}}`: IMEI of the device
- `{{mail}}`: Email address of the user
- `{{MEID}}`: MEID of the device
- `{{partialUPN}}`: UPN prefix before the `@` symbol
- `{{SerialNumber}}`: Device serial number
- `{{SerialNumberLast4Digits}}`: Last four digits of the device serial number
- `{{UserId}}`: Intune user ID
- `{{UserName}}`: User name
- `{{userPrincipalName}}`: UPN of the user

> [!NOTE]
> Variables aren't validated in the UI and are case sensitive. As a result, you may see profiles saved with incorrect input. For example, if you enter `{{DeviceID}}`, instead of `{{deviceid}}` or `{{DEVICEID}}`, then the literal string is shown instead of the device's unique ID. Be sure to enter the correct information. All lowercase or all uppercase variables are supported, but not a mix.

For more information on this setting, go to [Android Enterprise device settings to allow or restrict features using Intune](../configuration/device-restrictions-android-for-work.md#custom-support-information).

Applies to:
- Android 7.0 and newer
- Android Enterprise corporate owned fully managed
- Android Enterprise corporate owned dedicated devices
- Android Enterprise corporate owned work profile

#### Filter on the user scope or device scope in the settings catalog for Windows devices<!-- 13949975 -->
When you create a settings catalog policy, you can use **Add settings** > **Add filter** to filter settings based on the Windows OS edition (**Devices** > **Configuration profiles** > **Create profile** > **Windows 10 and later** for platform > **Settings catalog** for profile type).

When you **Add filter**, you can also filter on the settings by user scope or device scope.

For more information on the settings catalog, go to [Use the settings catalog to configure settings on Windows, iOS/iPadOS and macOS devices](../configuration/settings-catalog.md).

Applies to:
- Windows 10
- Windows 11

#### Android Open Source Project (AOSP) platform is generally available<!-- 15027949 -->
Microsoft Intune management of corporate-owned devices that run on the Android Open Source Project (AOSP) platform is now generally available (GA). This includes the full suite of capabilities that have been made available as part of the public preview.

Currently, Microsoft Intune only supports the new Android (AOSP) management option for RealWear devices.
- [Deployment guide: Manage Android devices in Microsoft Intune](deployment-guide-platform-android.md)
- [Deployment guide: Enroll Android devices in Microsoft Intune](deployment-guide-enrollment-android.md)

Applies to:
- Android Open Source Project (AOSP)

#### Device Firmware Configuration Interface (DFCI) now supports Acer devices<!-- 15240661 -->
For Windows 10/11 devices, you can create a DFCI profile to manage UEFI (BIOS) settings (**Devices** > **Configuration profiles** > **Create profile** > **Windows 10 and later** for platform > **Templates** > **Device Firmware Configuration Interface** for profile type).

New Acer devices running Windows 10/11 will be enabled for DFCI in later 2022. So, admins can create DFCI profiles to manage the BIOS and then deploy the profiles to these Acer devices.

Contact your device vendor or device manufacturer to ensure you get eligible devices.

For more information about DFCI profiles in Intune, go to [Use Device Firmware Configuration Interface (DFCI) profiles on Windows devices in Microsoft Intune](../configuration/device-firmware-configuration-interface-windows.md).

Applies to:
- Windows 10
- Windows 11

#### New settings available in the iOS/iPadOS and macOS settings catalog<!-- 15349701 -->
The [settings catalog](../configuration/settings-catalog.md) lists all the settings you can configure in a device policy, and all in one place. 

There are new settings available in the settings catalog. In the [Microsoft Endpoint Manager admin center](https://go.microsoft.com/fwlink/?linkid=2109431), you can see these settings at **Devices** > **Configuration profiles** > **Create profile** > **iOS/iPadOS** or **macOS** for platform > **Settings catalog** for profile type.

New settings include:

**Accounts > LDAP**:

- LDAP Account Description
- LDAP Account Host Name
- LDAP Account Password
- LDAP Account Use SSL
- LDAP Account User Name
- LDAP Search Settings

Applies to:
- iOS/iPadOS
- macOS

The following settings are also in settings catalog. Previously, they were only available in Templates:

**Privacy > Privacy Preferences Policy Control**:

- Accessibility
- Address Book
- Apple Events
- Calendar
- Camera
- File Provider Presence
- Listen Event
- Media Library
- Microphone
- Photos
- Post Event
- Reminders
- Screen Capture
- Speech Recognition
- System Policy All Files
- System Policy Desktop Folder
- System Policy Documents Folder
- System Policy Downloads Folder
- System Policy Network Volumes
- System Policy Removable Volumes
- System Policy Sys Admin Files

Applies to:

- macOS

For more information about configuring settings catalog profiles in Intune, see [Create a policy using settings catalog](../configuration/settings-catalog.md).

### Device enrollment

#### Set up enrollment notifications (public preview)<!-- 9283605 -->
Enrollment notifications inform device users, via email or push notification, when a new device has been enrolled in Microsoft Intune. You can use enrollment notifications for security purposes to notify users and help them report devices enrolled in error, or for communicating to employees during the hiring or onboarding process. Enrollment notifications are available to try now in public preview for Windows, Apple, and Android devices. This feature is only supported with user-driven enrollment methods.

### Device security

#### Assign compliance policies to the All devices group<!-- 2213410 -->
The **All devices** option is now available for [compliance policy](../protect/create-compliance-policy.md) assignments. With this option you can assign a compliance policy to all enrolled devices in your organization that match the policy's platform, without needing to create an Azure Active Directory group that contains all devices. 
 
When you include the *All devices* group you can then exclude individual groups of devices to further refine the assignment scope.

#### Trend Micro – New mobile threat defense partner<!-- 11017779 -->
You can now use [Trend Micro Mobile Security as a Service](../protect/trend-micro-mobile-threat-defense-connector.md) as an integrated mobile threat defense (MTD) partner with Intune. By configuring the Trend MTD connector in Intune, you can control mobile device access to corporate resources using conditional access that's based on risk assessment.
 
For more information, see:
- [Mobile threat defense integration with Intune](../protect/mobile-threat-defense.md)
- [Trend Micro Mobile Security documentation](https://docs.trendmicro.com/en-us/enterprise/trend-micro-vision-one/mobile-security/getting-started-with_003.aspx)

#### Grace period status visible on Intune Company Portal website<!-- 15025900 -->
The Intune Company Portal website now shows a grace period status to account for devices that don't meet compliance requirements but are still within their given grace period. Users are shown the date by which they need to become compliant and the instructions for how to become compliant. If they don't update their device by the given date, their status changes to noncompliant. For more information about setting grace periods, see [Configure compliance policies with actions for noncompliance](../protect/actions-for-noncompliance.md#available-actions-for-noncompliance).

### Intune apps

#### Newly available protected apps for Intune<!-- 15007580, 15235927 -->
The following protected apps are now available for Microsoft Intune:
- RingCentral for Intune by RingCentral, Inc.
- MangoApps, Work from Anywhere by MangoSpring, Inc.

For more information about protected apps, see [Microsoft Intune protected apps](../apps/apps-supported-intune-apps.md).

## Week of September 12, 2022

### Device management

#### Intune now requires iOS/iPadOS 14 and higher<!-- 14778947 -->
With Apple's release of iOS/iPadOS 16, Microsoft Intune and the Intune Company Portal will now require iOS/iPadOS 14 and higher. For related information, see [Supported operating systems and browsers in Intune](../fundamentals/supported-devices-browsers.md).

#### Intune now requires macOS 11.6 and higher<!-- 14766663 -->
With Apple's release of macOS 13 Ventura, Microsoft Intune, the Company Portal app, and the Intune MDM agent will now require macOS 11.6 (Big Sur) and later. For related information, see [Supported operating systems and browsers in Intune](../fundamentals/supported-devices-browsers.md).

## Week of September 05, 2022

### Device management

#### Remote Help version: 4.0.1.13 release<!-- 15329690 -->

With Remote Help 4.0.1.13 fixes were introduced to address an issue that prevented people from having multiple sessions open at the same time. The fixes also addressed an issue where the app was launching without focus, and prevented keyboard navigation and screen readers from working on launch.

For more information, go to [Use Remote Help with Intune and Microsoft Endpoint Manager](../remote-actions/remote-help.md)

## Week of August 29, 2022

### App management

#### Updated Microsoft Intune App SDK for Android<!-- 15363982 -->
The developer guide for the Intune App SDK for Android has been updated. The updated guide provides the following stages:
- Planning the integration
- MSAL prerequisite
- Getting started with MAM
- MAM integration essentials
- Multi-Identity
- App configuration
- App participation features

For more information, see [Intune App SDK for Android](../developer/app-sdk-android-phase1.md).

## Week of August 22, 2022

### Device management

#### Use Intune role-based access control (RBAC) for tenant attached devices <!-- 14996522 -->

You can now use Intune role-based access control (RBAC) when interacting with tenant attached devices from the Microsoft Endpoint Manager admin center. For example, when using Intune as the role-based access control authority, a user with Intune's [Help Desk Operator role](role-based-access-control.md#built-in-roles) doesn't need an assigned security role or additional permissions from Configuration Manager. For more information, see [Intune role-based access control for tenant attached clients](../../configmgr/cloud-attach/use-intune-rbac.md).

## Week of August 15, 2022 (Service release 2208)

### App management

#### Android strong biometric change detection<!-- 9740832 -->
The Android **Fingerprint instead of PIN for access** setting in Intune, which allows the end-user to use [fingerprint authentication](https://developer.android.com/about/versions/marshmallow/android-6.0.html#fingerprint-authentication) instead of a PIN, is being modified. This change will allow you to require end-users to set strong biometrics, as well as require end-users to confirm their app protection policy (APP) PIN if a change in strong biometrics is detected. You can find Android app protection polices in [Microsoft Endpoint Manager admin center](https://go.microsoft.com/fwlink/?linkid=2109431) by selecting **Apps** > **App protection policies** > **Create policy** > **Android**. For more information, see [Android app protection policy settings in Microsoft Intune](../apps/app-protection-policy-settings-android.md#access-requirements).

#### Noncompliance details available for Android (AOSP) in Microsoft Intune app<!-- 12645770 -->
Android (AOSP) users can view noncompliance reasons in the Microsoft Intune app. These details describe why a device is marked noncompliant, and are available on the Device details page for devices enrolled as user-associated Android (AOSP) devices.  

### Intune apps

#### Newly available protected apps for Intune<!-- 14709109, 14955442, 14981985 -->
The following protected apps are now available for Microsoft Intune:
- Nexis Newsdesk Mobile by LexisNexis
- My Portal by MangoApps (Android)
- Re:Work Enterprise by 9Folders, Inc.

For more information about protected apps, see [Microsoft Intune protected apps](../apps/apps-supported-intune-apps.md).

### Device enrollment

#### Configure zero-touch enrollment from Microsoft Endpoint Manager admin center<!-- 1872357 -->
Now you can configure Android zero-touch enrollment from the [Microsoft Endpoint Manager admin center](https://go.microsoft.com/fwlink/?linkid=2109431). This feature lets you link your zero-touch account to Intune, add support information, configure zero-touch enabled devices, and customize provisioning extras. For more information about how to enable zero-touch from the admin center, see [Enroll by using Google Zero Touch](../enrollment/android-dedicated-devices-fully-managed-enroll.md#enroll-by-using-google-zero-touch).  

### Device management

#### Custom settings for Windows 10/11 device compliance is now generally available<!-- 12862904 -->
Support to [create custom compliance policy settings](../protect/compliance-use-custom-settings.md) for Windows devices using PowerShell scripts, and to create custom compliance rules and remediation messages that appear in the Company Portal, is now generally available.

Applies to:  
- Windows 10/11

#### View contents of macOS shell scripts and custom attributes<!-- 14757037 -->
You can view the contents of macOS shell scripts and custom attributes after you upload these to Intune. You can view Shell scripts and custom attributes in [Microsoft Endpoint Manager admin center](https://go.microsoft.com/fwlink/?linkid=2109431) by selecting **Devices** > **macOS**. For related information, see [Use shell scripts on macOS devices in Intune](../apps/macos-shell-scripts.md).

#### Reset passcode remote action available for Android (AOSP) Corporate devices<!-- 10247332 -->
You'll be able to leverage Reset passcode remote action from the [Microsoft Endpoint Manager admin center](https://go.microsoft.com/fwlink/?linkid=2109431) for Android Open Source Project (AOSP) Corporate devices.

For information on remote actions, see:
- [Reset or remove a device passcode in Intune](../remote-actions/device-passcode-reset.md)
- [Remotely restart devices with Intune](../remote-actions/device-restart.md)
- [Remotely lock devices with Intune](../remote-actions/device-remote-lock.md)

Applies to:
- Android Open Source Project (AOSP)

### Device configuration

#### Certificate profiles support for Android (ASOP) devices<!-- 8506336 -->
You can now use Simple Certificate Enrollment Protocol (SCEP) [certificate profiles](../protect/certificates-configure.md) with corporate-owned and userless devices that run the Android Open Source Project (AOSP) platform.

#### Import, create, and manage custom ADMX and ADML administrative templates<!-- 4970862 -->
You can create a device configuration policy that uses built-in ADMX templates. In [Microsoft Endpoint Manager admin center](https://go.microsoft.com/fwlink/?linkid=2109431), select **Devices** > **Configuration profiles** > **Create profile** > **Windows 10 and later** for platform > **Templates** > **Administrative templates**.

You can also import custom and third party/partner ADMX and ADML templates into the Endpoint Manager admin center. Once imported, you can create a device configuration policy, assign the policy to your devices, and manage the settings in the policy.

For information, go to:
- [Import custom ADMX and ADML administrative templates into Endpoint Manager](../configuration/administrative-templates-import-custom.md)
- [Overview: Use Windows 10/11 templates to configure group policy settings in Microsoft Intune](../configuration/administrative-templates-windows.md).

Applies to:
- Windows 11
- Windows 10

#### Add an HTTP proxy to Wi-Fi device configuration profiles on Android Enterprise<!-- 13975609 -->
On Android Enterprise devices, you can create a Wi-Fi device configuration profile with basic and enterprise settings. In [Microsoft Endpoint Manager admin center](https://go.microsoft.com/fwlink/?linkid=2109431), select **Devices** > **Configuration profiles** > **Create profile** > **Android Enterprise** > **Fully Managed, Dedicated, and Corporate-Owned Work Profile** for platform > **Wi-Fi**.

When you create the profile, you can configure an HTTP proxy using a PAC file or configure the settings manually. You can configure an HTTP proxy for each Wi-Fi network in your organization.

When the profile is ready, you can deploy this profile to your Fully Managed, Dedicated, and Corporate-Owned Work Profile devices. 

For more information on the Wi-Fi settings you can configure, go to [Add Wi-Fi settings for Android Enterprise dedicated and fully managed devices in Microsoft Intune](../configuration/wi-fi-settings-android-enterprise.md).

Applies to:
- Android Enterprise Fully Managed, Dedicated, and Corporate-Owned Work Profile

#### iOS/iPadOS settings catalog supports declarative device management (DDM)<!-- 15016105 -->
On iOS/iPadOS 15+ devices enrolled using [User Enrollment](../enrollment/ios-user-enrollment.md), the settings catalog automatically uses Apple’s declarative device management (DDM) when configuring settings.
- No action is required to use DDM. The feature is built into the settings catalog.
- There is no impact to existing policies in the settings catalog.
- iOS/iPadOS devices that aren't enabled for DDM continue to use Apple’s standard MDM protocol.

For more information, go to:
- [Meet declarative device management](https://aka.ms/DDM2021) (opens Apple's web site)
- [Microsoft simplifies Endpoint Manager enrollment for Apple updates](https://techcommunity.microsoft.com/t5/microsoft-endpoint-manager-blog/microsoft-simplifies-endpoint-manager-enrollment-for-apple/ba-p/3570319)
- [Use the settings catalog to configure settings on Windows, iOS/iPadOS and macOS devices](../configuration/settings-catalog.md)

Applies to:
-  iOS/iPadOS 15 or later devices enrolled using Apple User Enrollment

#### New macOS settings available in the settings catalog <!-- 15020250 -->
The [settings catalog](../configuration/settings-catalog.md) lists all the settings you can configure in a device policy, and all in one place. New settings are available in the settings catalog. In [Microsoft Endpoint Manager admin center](https://go.microsoft.com/fwlink/?linkid=2109431), select **Devices** > **Configuration profiles** > **Create profile** > **macOS** for platform > **Settings catalog** for profile type.

New settings include:

**Microsoft Auto Update**:

- Current Channel
- Number of minutes for the final countdown timer

**Restrictions**:

- Allow Universal Control

The following settings are also in settings catalog. Previously, they were only available in Templates:

**Authentication > Extensible Single Sign On**:

- Extension Data
- Extension Identifier
- Hosts
- Realm
- Screen Locked Behavior
- Team Identifier
- Type
- URLs

**Authentication > Extensible Single Sign On > Extensible Single Sign On Kerberos**:

- Extension Data
- Allow Automatic Login
- Allow Password Change
- Credential Bundle ID ACL
- Credential Use Mode
- Custom Username Label
- Delay User Setup
- Domain Realm Mapping
- Help Text
- Include Kerberos Apps In Bundle ID ACL
- Include Managed Apps In Bundle ID ACL
- Is Default Realm
- Monitor Credentials Cache
- Perform Kerberos Only
- Preferred KDCs
- Principal Name
- Password Change URL
- Password Notification Days
- Password Req Complexity
- Password Req History
- Password Req Length
- Password Req Min Age
- Password Req Text
- Require TLS For LDAP
- Require User Presence
- Site Code
- Sync Local Password
- Use Site Auto Discovery
- Extension Identifier
- Hosts
- Realm
- Team Identifier
- Type

For more information about configuring settings catalog profiles in Intune, see [Create a policy using settings catalog](../configuration/settings-catalog.md).

Applies to:
- macOS

#### New iOS/iPadOS settings in the settings catalog<!-- 15020319 -->
The [settings catalog](../configuration/settings-catalog.md) lists all the settings you can configure in a device policy, and all in one place. There are new iOS/iPadOS settings available in the settings catalog. In [Microsoft Endpoint Manager admin center](https://go.microsoft.com/fwlink/?linkid=2109431), select **Devices** > **Configuration profiles** > **Create profile** > **iOS/iPadOS** for platform > **Settings catalog** for profile type. Previously, these settings were only available in Templates:

**Authentication > Extensible Single Sign On**:

- Extension Data
- Extension Identifier
- Hosts
- Realm
- Screen Locked Behavior
- Team Identifier
- Type
- URLs

**Authentication > Extensible Single Sign On > Extensible Single Sign On Kerberos**:

- Extension Data
- Allow Automatic Login
- Credential Bundle ID ACL
- Domain Realm Mapping
- Help Text
- Include Managed Apps In Bundle ID ACL
- Is Default Realm
- Preferred KDCs
- Principal Name
- Require User Presence
- Site Code
- Use Site Auto Discovery
- Extension Identifier
- Hosts
- Realm
- Team Identifier
- Type

**System Configuration > Lock Screen Message**:
- Asset Tag Information
- Lock Screen Footnote

For more information about configuring settings catalog profiles in Intune, see [Create a policy using settings catalog](../configuration/settings-catalog.md).

Applies to:
- iOS/iPadOS

### Monitor and troubleshoot

#### New noncompliant devices and settings report<!-- 13532817 -->
In **Reports** > **Device Compliance** > **Reports**, there's a new **Noncompliant devices and settings** organization report. This report:
- Lists each noncompliant device.
- For each noncompliant device, it shows the compliance policy settings that the devices aren't compliant with.

For more information on this report, go to [Noncompliant devices and settings report (Organizational)](reports.md#noncompliant-devices-and-settings-report-organizational).

## Week of August 1, 2022

### Device security

#### Disable use of UDP connections on your Microsoft Tunnel Gateway servers<!-- 9295335 -->

You can now disable the use of UDP by your Microsoft Tunnel Servers. When you disable use of UDP, the VPN server supports only TCP connections from tunnel clients. To support use of only TCP connections, your devices must use the generally available version of [Microsoft Defender for Endpoint as the Microsoft Tunnel client app](../protect/microsoft-tunnel-migrate-app.md) as the tunnel client app.

To disable UDP, [create or edit a *Server configuration* for Microsoft Tunnel Gateway](../protect/microsoft-tunnel-configure.md#create-a-server-configuration) and select the checkbox for the new option named **Disable UDP Connections**.

### App management

#### Company Portal for Windows bulk app install<!-- 6401437 -->
The Company Portal for Windows now allows users to select multiple apps and install in bulk. From the **Apps** tab of the Company Portal for Windows, select the multi-select view button on the top right corner of the page. Then, select the checkbox next to each app that you need to install. Next, select the **Install Selected** button to start installation. All selected apps will install at the same time without requiring users to right-click each app or navigate to each app's page. For related information, see [Install and share apps on your device](../user-help/install-apps-cpapp-windows.md) and [How to configure the Intune Company Portal apps, Company Portal website, and Intune app](../apps/company-portal-app.md).

## Week of July 25, 2022 (Service release 2207)

### Device management

#### Initiate compliance checks for your AOSP devices from the Microsoft Intune app<!--12645739 -->
You can now initiate a compliance check for your AOSP devices from the Microsoft Intune app. Go to **Device details**. This feature is available on devices that are enrolled via the Microsoft Intune app as user-associated (Android) AOSP devices.

#### Monitor bootstrap escrow status on a Mac<!-- 12404441 -->  
Monitor the bootstrap token escrow status for an enrolled Mac in the [Microsoft Endpoint Manager admin center](https://go.microsoft.com/fwlink/?linkid=2109431). A new hardware property in Intune, called *Bootstrap token escrowed*, reports whether or not a bootstrap token has been escrowed in Intune. For more information about bootstrap token support for macOS, see [Bootstrap tokens](../enrollment/macos-enroll.md#bootstrap-tokens).

#### Enable Common Criteria mode for Android Enterprise devices<!-- 13158881 -->
For Android Enterprise devices, you can use a new setting, **Common Criteria mode**, to enable an elevated set of security standards that are typically used by only highly sensitive organizations, such as government establishments.

Applies to:
- Android 5.0 and newer
- Android Enterprise corporate owned fully managed
- Android Enterprise corporate owned dedicated devices
- Android Enterprise corporate owned work profile

The new setting, *Common Criteria mode*, is found in the *System security* category when you configure a [Device restrictions](../configuration/device-restrictions-configure.md) template for the *Android Enterprise - Fully Managed, Dedicated, and Corporate-Owned Work Profile*.
 
Devices that receive a policy with *Common Criteria mode* set to **Require**, elevate security components that include but are not limited to:  
- AES-GCM encryption of Bluetooth Long Term Keys
- Wi-Fi configuration stores
- Blocks bootloader download mode, the manual method for software updates
- Mandates additional key zeroization on key deletion
- Prevents non-authenticated Bluetooth connections
- Requires that FOTA updates have 2048-bit RSA-PSS signature

Learn more about Common Criteria:
- [Common Criteria for Information Technology Security Evaluation](https://www.commoncriteriaportal.org) at commoncriteriaportal.org
- [CommonCriteriaMode](https://developers.google.com/android/management/reference/rest/v1/enterprises.policies#commoncriteriamode) in the Android Management API documentation
- [Knox Deep Dive: Common Criteria Mode](https://www.samsungknox.com/blog/knox-deep-dive-common-criteria-mode) at samsungknox.com

#### New hardware detail available for individual devices running on iOS/iPadOS and macOS<!-- 9598434 -->
In [Microsoft Endpoint Manager admin center](https://go.microsoft.com/fwlink/?linkid=2109431), select **Devices** > **All devices** > *select one of your listed devices* and open it's **Hardware** details. The following new detail is available in the **Hardware** pane of individual devices:
 - **Product name**: Shows the product name of the device, such as iPad8,12. Available for iOS/iPadOS and macOS devices. 

For more information, see [View device details with Microsoft Intune](../remote-actions/device-inventory.md).

Applies to:
- iOS/iPadOS, macOS

#### Remote Help Version: 4.0.1.12 release<!-- 14999203 -->
With Remote Help 4.0.1.12 various fixes were introduced to address the 'Try again later' message that appears when not authenticated. The fixes also include an improved auto-update capability. 

For more information, see [Use Remote Help with Intune and Microsoft Endpoint Manager](../remote-actions/remote-help.md)

### Device enrollment

#### Intune supports sign-in from another device during iOS/iPadOS and macOS Setup Assistant with modern authentication<!-- 12377183 -->  
Users going through automated device enrollment (ADE) can now authenticate by signing in from another device. This option is available for iOS/iPadOS and macOS devices enrolling via Setup Assistant with modern authentication. The screen that prompts device users to sign in from another device is embedded into Setup Assistant and shown to them during enrollment. For more information about the sign-in process for users, see [Get the Intune Company Portal app (../user-help/sign-in-to-the-company-portal.md#sign-in-via-another-device).  

#### Detect and manage hardware changes on Windows Autopilot devices<!-- 12795465 --> 
Microsoft Intune will now alert you when it detects a hardware change on an Autopilot-registered device. You can view and manage all affected devices in the admin center. Additionally, you have the option to remove the affected device from Windows Autopilot and register it again so that the hardware change is accounted for.

### Device configuration

#### New macOS Microsoft AutoUpdate (MAU) settings in the settings catalog<!-- 14873468 -->
The settings catalog supports settings for Microsoft AutoUpdate (MAU) (**Devices** > **Configuration profiles** > **Create profile** > **macOS** for platform >**Settings catalog** for profile type).

The following settings are now available:

**Microsoft Auto Update**:

- Automatically acknowledge data collection policy
- Days before forced updates
- Deferred updates
- Disable Office Insider membership
- Enable AutoUpdate
- Enable check for updates
- Enable extended logging
- Register app on launch
- Update cache server
- Update channel
- Update check frequency (mins)
- Updater optimization technique

The settings can be used to configure preferences for the following applications:

- Company Portal
- Microsoft Auto Update
- Microsoft Defender
- Microsoft Defender ATP
- Microsoft Edge
- Microsoft Edge Beta
- Microsoft Edge Canary
- Microsoft Edge Dev
- Microsoft Excel
- Microsoft OneNote
- Microsoft Outlook
- Microsoft PowerPoint
- Microsoft Remote Desktop
- Microsoft Teams
- Microsoft Word
- OneDrive
- Skype for Business

For more information about the settings catalog, go to:
- [Tasks you can complete using the Settings Catalog in Intune](../configuration/settings-catalog-common-features.md)
- [Create a policy using settings catalog in Microsoft Intune](../configuration/settings-catalog.md)

For more information about Microsoft AutoUpdate settings you can configure, go to:
- [Use preferences to manage privacy controls for Office for Mac - Deploy Office](/deployoffice/privacy/mac-privacy-preferences#preference-setting-for-connected-experiences-that-download-online-content).
- [Set a deadline for updates from Microsoft AutoUpdate](/deployoffice/mac/mau-deadline)

Applies to:
- macOS

#### New iOS/iPadOS settings in the settings catalog<!-- 14875716 -->
The [settings catalog](../configuration/settings-catalog.md) lists all the settings you can configure in a device policy, and all in one place. There are new iOS/iPadOS settings available in the settings catalog (**Devices** > **Configuration profiles** > **Create profile** > **iOS/iPadOS** for platform > **Settings catalog** for profile type).

New settings include:

**Networking > Cellular**:
- Allowed Protocol Mask
- Allowed Protocol Mask In Domestic Roaming
- Allowed Protocol Mask In Roaming
- Authentication Type
- Name
- Password
- Proxy Port
- Proxy Server
- Username

The following settings are also in settings catalog. Previously, they were only available in Templates:

**User experience > Notifications**:
- Grouping type
- Preview type
- Show In Car Play

**Printing > Air Print**:
- Force TLS
- Port

**App Management > App Lock**:
- Disable Auto Lock
- Disable Device Rotation
- Disable Ringer Switch
- Disable Sleep Wake Button
- Disable Touch
- Disable Volume Buttons
- Enable Assistive Touch
- Enable Invert Colors
- Enable Mono Audio
- Enable Speak Selection
- Enable Voice Control
- Enable Voice Over
- Enable Zoom
- Assistive Touch
- Invert Colors
- Voice Control
- Voice Over
- Zoom

**Networking > Domains**:
- Safari Password Auto Fill Domain

**Networking > Network Usage Rules**:
- Application Rules
- Allow Cellular Data
- Allow Roaming Cellular Data
- App Identifier Matches

**Restrictions**:
- Allow Account Modification
- Allow Activity Continuation
- Allow Adding Game Center Friends
- Allow Air Drop
- Allow Air Print
- Allow Air Print Credentials Storage
- Allow Air Print iBeacon Discovery
- Allow App Cellular Data Modification
- Allow App Clips
- Allow App Installation
- Allow App Removal
- Allow Apple Personalized Advertising
- Allow Assistant
- Allow Assistant User Generated Content
- Allow Assistant While Locked
- Allow Auto Correction
- Allow Auto Unlock
- Allow Automatic App Downloads
- Allow Bluetooth Modification
- Allow Bookstore
- Allow Bookstore Erotica
- Allow Camera
- Allow Cellular Plan Modification
- Allow Chat
- Allow Cloud Backup
- Allow Cloud Document Sync
- Allow Cloud Keychain Sync
- Allow Cloud Photo Library
- Allow Cloud Private Relay
- Allow Continuous Path Keyboard
- Allow Definition Lookup
- Allow Device Name Modification
- Allow Diagnostic Submission
- Allow Diagnostic Submission Modification
- Allow Dictation
- Allow Enabling Restrictions
- Allow Enterprise App Trust
- Allow Enterprise Book Backup
- Allow Enterprise Book Metadata Sync
- Allow Erase Content And Settings
- Allow ESIM Modification
- Allow Explicit Content
- Allow Files Network Drive Access
- Allow Files USB Drive Access
- Allow Find My Device
- Allow Find My Friends
- Allow Find My Friends Modification
- Allow Fingerprint For Unlock
- Allow Fingerprint Modification
- Allow Game Center
- Allow Global Background Fetch When Roaming
- Allow Host Pairing
- Allow In App Purchases
- Allow iTunes
- Allow Keyboard Shortcuts
- Allow Listed App Bundle IDs
- Allow Lock Screen Control Center
- Allow Lock Screen Notifications View
- Allow Lock Screen Today View
- Allow Mail Privacy Protection
- Allow Managed Apps Cloud Sync
- Allow Managed To Write Unmanaged Contacts
- Allow Multiplayer Gaming
- Allow Music Service
- Allow News
- Allow NFC
- Allow Notifications Modification
- Allow Open From Managed To Unmanaged
- Allow Open From Unmanaged To Managed
- Allow OTAPKI Updates
- Allow Paired Watch
- Allow Passbook While Locked
- Allow Passcode Modification
- Allow Password Auto Fill
- Allow Password Proximity Requests
- Allow Password Sharing
- Allow Personal Hotspot Modification
- Allow Photo Stream
- Allow Podcasts
- Allow Predictive Keyboard
- Allow Proximity Setup To New Device
- Allow Radio Service
- Allow Remote Screen Observation
- Allow Safari
- Allow Screenshot
- Allow Shared Device Temporary Session
- Allow Shared Stream
- Allow Spell Check
- Allow Spotlight Internet Results
- Allow System App Removal
- Allow UI App Installation
- Allow UI Configuration Profile Installation
- Allow Unmanaged To Read Managed Contacts
- Allow Unpaired External Boot To Recovery
- Allow Untrusted TLS Prompt
- Allow USB Restricted Mode
- Allow Video Conferencing
- Allow Voice Dialing
- Allow VPN Creation
- Allow Wallpaper Modification
- Autonomous Single App Mode Permitted App IDs
- Blocked App Bundle IDs
- Enforced Software Update Delay
- Force Air Drop Unmanaged
- Force Air Play Outgoing Requests Pairing Password
- Force Air Print Trusted TLS Requirement
- Force Assistant Profanity Filter
- Force Authentication Before Auto Fill
- Force Automatic Date And Time
- Force Classroom Automatically Join Classes
- Force Classroom Request Permission To Leave Classes
- Force Classroom Unprompted App And Device Lock
- Force Delayed Software Updates
- Force Encrypted Backup
- Force iTunes Store Password Entry
- Force Limit Ad Tracking
- Force On Device Only Dictation
- Force On Device Only Translation
- Force Watch Wrist Detection
- Force WiFi Power On
- Force WiFi To Allowed Networks Only
- Require Managed Pasteboard
- Safari Accept Cookies
- Safari Allow Autofill
- Safari Allow JavaScript
- Safari Allow Popups
- Safari Force Fraud Warning

For more information about configuring Settings catalog profiles in Intune, see [Create a policy using settings catalog](../configuration/settings-catalog.md).

Applies to:
- iOS/iPadOS

#### New macOS settings available in the settings catalog<!-- 14875745 -->
The [settings catalog](../configuration/settings-catalog.md) lists all the settings you can configure in a device policy, and all in one place. New settings are available in the settings catalog (**Devices** > **Configuration profiles** > **Create profile** > **macOS** for platform > **Settings catalog** for profile type).

New settings include:

**System configuration > System extensions**:

- Removable System Extensions

The following settings are also in settings catalog. Previously, they were only available in Templates:

**System configuration > System extensions**:
- Allow User Overrides
- Allowed System Extension Types
- Allowed System Extensions
- Allowed Team Identifiers

For more information about configuring settings catalog profiles in Intune, see [Create a policy using settings catalog](../configuration/settings-catalog.md).

Applies to:
- macOS

#### New search feature in Preview devices when creating a filter<!-- 14921046 -->
In [Microsoft Endpoint Manager admin center](https://go.microsoft.com/fwlink/?linkid=2109431), you can create filters, and then use these filters when assigning apps and policies (**Devices** > **Filters** > **Create**).

When you create a filter, you can select **Preview devices** to see a list of enrolled devices that match your filter criteria. In **Preview devices**, you can also search through the list using the device name, OS version, device model, device manufacturer, user principal name of the primary user, and device ID.

For more information on filters, go to [Use filters when assigning your apps, policies, and profiles in Microsoft Endpoint Manager](../fundamentals/filters.md).

## Week of July 18, 2022

### Device management

#### New event viewers to assist in debugging WMI issues<!-- 14712854  -->
Intune’s remote action to [collect diagnostics](../remote-actions/collect-diagnostics.md#collect-diagnostics) has been expanded to collect details about Windows Management Instrumentation (WMI) app issues.

The new event viewers include the following:
- Microsoft-Windows-WMI-Activity/Operational
- Microsoft-Windows-WinRM/Operational

For more information about Windows device diagnostics, see [Collect diagnostics from a Windows device](../remote-actions/collect-diagnostics.md).

## Week of July 4, 2022

### Device management

#### Endpoint analytics scores per device model<!-- 14439211 -->

Endpoint analytics now displays [scores by device model](../../analytics/scores.md#bkmk_model). These scores help admins contextualize the user experience across device models in the environment. Scores per model and per device are available in all Endpoint analytics reports, including the [Work from anywhere](../../analytics/work-from-anywhere.md) report.

### Monitor and troubleshoot

#### Use Collect diagnostics to collect details about Windows expedited updates<!--  14337387 -->

Intune’s remote action to [Collect diagnostics](../remote-actions/collect-diagnostics.md) now collects additional details about [Windows expedited updates](../protect/windows-10-expedite-updates.md) that you deploy to devices. This information can be of use when troubleshooting problems with expedited updates.

The new details that are collected include:  
- Files: `C:\Program Files\Microsoft Update Health Tools\Logs\*.etl`
- Registry Keys: `HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\CloudManagedUpdate`


## Week of June 27, 2022 (Service release 2206)

### App management

#### Enterprise feedback policies for Web Company Portal<!-- 9846764 -->
Feedback settings are now available to address M365 enterprise feedback policies for the currently logged in user via the [Microsoft 365 Apps admin center](https://config.office.com/). The settings are used to determine whether feedback can be enabled or must be disabled for a user in the Web Company Portal. For related information, see [Configure feedback settings for Company Portal and Microsoft Intune apps](../apps/company-portal-app.md#configure-feedback-settings-for-company-portal-and-microsoft-intune-apps).

#### App Protection Policies with Android Enterprise dedicated devices and Android (AOSP) devices<!-- 13819227 -->
Intune-managed Android Enterprise dedicated devices enrolled with Azure Active Directory (Azure AD) shared mode and Android (AOSP) devices can now receive app protection policies and can be targeted separately from other Android device types. For related information, see [Add Managed Google Play apps to Android Enterprise devices with Intune](../apps/apps-add-android-for-work.md). For more information about Android Enterprise dedicated devices and Android (AOSP), see [Android Enterprise dedicated devices](../fundamentals/deployment-guide-enrollment-android.md#android-enterprise-dedicated-devices).

### Device security

#### Users assigned the Endpoint Security Manager admin role can modify Mobile Threat Defense connector settings<!-- 14179885 -->
We’ve updated the permissions of the built-in [Endpoint Security Manager](../fundamentals/role-based-access-control.md#built-in-roles) admin role. The role now has the **Modify** permission for the **Mobile Threat Defense** category set to **Yes**. With this change, users assigned this role have permission to change the [Mobile Threat Defense connector](../protect/mtd-connector-enable.md) (MTD connector) settings for your Tenant. Previously, this permission was set to *No*.

If you missed the previous notice about this coming change, now is a good time to review the users that are assigned the *Endpoint Security Manager* role for your tenant. If any should not have permissions to edit the MTD connector settings, update their role permissions or [create a custom role](../fundamentals/create-custom-role.md) that includes only *Read* permissions for Mobile Threat Defense.

View the full list of permissions for the built-in [Endpoint Security Manager role](../protect/endpoint-security.md#permissions-granted-by-the-endpoint-security-manager-role).

#### Improved certificate profile support for Android Enterprise Fully Managed devices<!-- 14217083  -->
We’ve improved our [PKCS](../protect/certificates-pfx-configure.md) and [SCEP](../protect/certificates-profile-scep.md) certificate profile support for Android Enterprise Fully Managed (Device Owner) devices. You can now use the Intune device ID variable, **CN={{DeviceID}}**, as the subject alternative name (SAN) in your certificates for these devices. 

### Device configuration

### Certificate profiles support for Android (ASOP) devices<!-- 8506319, 8506363 -->
You can now use the following [certificate profiles](../protect/certificates-configure.md) with corporate-owned and userless devices that run the Android Open Source Project (AOSP) platform: 
- Trusted certificate profile
- PKCS certificate profile

#### New settings for DFCI profiles on Windows 10/11 devices<!-- 6039135 -->
On Windows 10/11 devices, you can create a Device Firmware Configuration Interface (DFCI) profile (**Devices** > **Configuration profiles** > **Create profile** > **Windows 10 and later** for platform > **Templates** > **Device Firmware Configuration Interface** for profile type).

DFCI profiles let Intune pass management commands to UEFI (Unified Extensible Firmware Interface) using the DFCI firmware layer. This additional firmware layer makes configuration more resilient to malicious attacks. DFCI also limits end users' control over the BIOS by graying out managed settings.

There are new settings you can configure:
- **Microphones and Speakers**:
  - Microphones

- **Radios**:
  - Bluetooth
  - Wi-Fi

- **Ports**:
  - USB type A

- **Wake settings**:
  - Wake on LAN
  - Wake on power

For more information, see the following resources:
- [Use Device Firmware Configuration Interface profiles on Windows devices in Microsoft Intune](../configuration/device-firmware-configuration-interface-windows.md)
- [Device Firmware Configuration Interface (DFCI) profile settings in Microsoft Intune](../configuration/device-firmware-configuration-interface-windows-settings.md)

Applies to:
- Windows 10/11

#### Add custom support information to Android Enterprise devices<!-- 7913128 -->
On Android Enterprise devices, you can create a device restrictions configuration profile that manages device settings (**Devices** > **Configuration profiles** > **Create profile** > **Android Enterprise** > **Fully managed, dedicated, and corporate-owned work profile** for platform > **Device restrictions** for profile type > **Custom support information**).

There are some new settings you can configure:
- **Short support message**: When users try to change a managed setting, you can add a short message that's shown to users in a system dialog window.
- **Long support message**: You can add a long message that's shown in **Settings** > **Security** > **Device admin apps** > **Device Policy**.

By default, the OEM default messages are shown. When you deploy a custom message, the Intune default message is also deployed. If you don't enter a custom message for the device's default language, then the Intune default message is shown. 

For example, you deploy a custom message for English and French. The user changes the device's default language to Spanish. Since you didn't deploy a custom message to the Spanish language, the Intune default message is shown.

The Intune default message is translated for all languages in the Endpoint Manger admin center (**Settings** > **Language + Region**). The **Language** setting value determines the default language used by Intune. By default, it's set to **English**.

In the policy, you can customize the messages for the following languages:
- Czech
- German
- English (United States)
- Spanish (Spain)
- French (France)
- Hungarian
- Indonesian
- Italian
- Japanese
- Korean
- Dutch
- Polish
- Portuguese (Brazil)
- Portuguese (Portugal)
- Russian
- Swedish
- Turkish
- Chinese (Simplified)
- Chinese (Traditional)

For more information on these settings and the other settings you can configure, go to [Android Enterprise device settings to allow or restrict features using Intune](../configuration/device-restrictions-android-for-work.md).

Applies to:
- Android 7.0 and newer
- Android Enterprise corporate owned fully managed (COBO)
- Android Enterprise corporate owned dedicated devices (COSU)
- Android Enterprise corporate owned work profile (COPE)

#### Create and deploy Wi-Fi profiles to Android AOSP devices<!-- 8506299 -->
You create configure and deploy a Wi-Fi profile to your Android AOSP devices.

For more information on these settings, go to [Add Wi-Fi settings for Android (AOSP) devices in Microsoft Intune](../configuration/wi-fi-settings-android-aosp.md).

Applies to:
- Android (AOSP)

#### Settings catalog is generally available (GA) for Windows and macOS devices<!-- 9558656 -->
The settings catalog is generally available (GA). For more information, go to:
- [Use the settings catalog to configure settings](../configuration/settings-catalog.md)
- [Tasks you can complete using the Settings Catalog in Intune](../configuration/settings-catalog-common-features.md)

Applies to:
- macOS
- Windows 10/11

#### Migrate feature in Group policy analytics supports sovereign clouds<!-- 13927582 -->
Using Group Policy analytics, you can import your on-premises GPOs, and create a settings catalog policy using these GPOs. Previously, this Migrate feature wasn't supported on Sovereign Clouds.

The Migrate feature is now supported on Sovereign Clouds.

For more information on these features, go to:
- [Analyze your on-premises GPOs using Group Policy analytics in Microsoft Endpoint Manager](../configuration/group-policy-analytics.md)
- [Create a Settings Catalog policy using your imported GPOs in Microsoft Endpoint Manager](../configuration/group-policy-analytics-migrate.md)

#### iOS/iPadOS platform is in settings catalog<!-- 13934066 -->
The [settings catalog](../configuration/settings-catalog.md) lists all the settings you can configure in a device policy, and all in one place. The iOS/iPadOS platform and some settings are now available in the settings catalog (**Devices** > **Configuration profiles** > **Create profile** > **iOS/iPadOS** for platform > **Settings catalog** for profile type).

New settings include:

**Accounts > Caldav**:

- Card DAV Account Description
- Card DAV Host Name
- Card DAV Password
- Card DAV Port
- Card DAV Principal URL
- Card DAV Use SSL
- Card DAV Username

**Accounts > Carddav**:

- Card DAV Account Description
- Card DAV Host Name
- Card DAV Password
- Card DAV Port
- Card DAV Principal URL
- Card DAV Use SSL
- Card DAV Username

**AirPlay**:

- Allow List
- Password

- **Profile Removal Password**:

- Removal Password

**Proxies > Global HTTP Proxy**:

- Proxy Captive Login Allowed
- Proxy PAC Fallback Allowed
- Proxy PAC URL
- Proxy Password
- Proxy Server
- Proxy Server Port
- Proxy Type
- Proxy Username

The following settings are also in Settings Catalog. Previously, they were only available in Templates:

**Networking > Domains**:

- Email Domains

**Printing > Air Print**:

- Printers
- IP Address
- Resource Path

**Restrictions**:

- Allow Activity Continuation
- Allow Adding Game Center Friends
- Allow Air Drop
- Allow Auto Unlock
- Allow Camera
- Allow Cloud Document Sync
- Allow Cloud Keychain Sync
- Allow Cloud Photo Library
- Allow Cloud Private Relay
- Allow Diagnostic Submission
- Allow Dictation
- Allow Erase Content And Settings
- Allow Fingerprint For Unlock
- Allow Game Center
- Allow Multiplayer Gaming
- Allow Music Service
- Allow Passcode Modification
- Allow Password Auto Fill
- Allow Password Proximity Requests
- Allow Password Sharing
- Allow Remote Screen Observation
- Allow Screenshot
- Allow Spotlight Internet Results
- Allow Wallpaper Modification
- Enforced Software Update Delay
- Force Classroom Automatically Join Classes
- Force Classroom Request Permission To Leave Classes
- Force Classroom Unprompted App And Device Lock
- Force Delayed Software Updates
- Safari Allow Autofill

**Security > Passcode**:

- Allow Simple Passcode
- Force PIN
- Max Failed Attempts
- Max Grace Period
- Max Inactivity
- Max PIN Age In Days
- Min Complex Characters
- Min Length
- PIN History
- Require Alphanumeric Passcode

**User Experience > Notifications**:

- Alert Type
- Badges Enabled
- Bundle Identifier
- Critical Alert Enabled
- Notifications Enabled
- Show In Lock Screen
- Show In Notification Center
- Sounds Enabled

For more information about configuring Settings catalog profiles in Intune, see [Create a policy using settings catalog](../configuration/settings-catalog.md).

Applies to:
- iOS/iPadOS

#### Use TEAP authentication in wired networks device configuration profiles for Windows devices<!-- 14042602 -->
On Windows devices, you can create a **Wired Networks** device configuration profile that supports the Extensible Authentication Protocol (EAP) (**Devices** > **Configuration profiles** > **Create profile** > **Windows 10 and later** for platform > **Templates** > **Wired networks** for profile type).

When you create the profile, you can use the Tunnel Extensible Authentication Protocol (TEAP).

For more information on wired networks, go to [Add and use wired networks settings on your macOS and Windows devices in Microsoft Intune](../configuration/wired-networks-configure.md).

Applies to:
- Windows 11
- Windows 10

#### Unlock the work profile on Android Enterprise corporate owned work profile (COPE) devices after a set time using password, PIN, or pattern<!-- 14133548 -->

On Android Enterprise devices, you can create a device restrictions configuration profile that manages device settings (**Devices** > **Configuration profiles** > **Create profile** > **Android Enterprise** > **Fully managed, dedicated, and corporate-owned work profile** for platform > **Device restrictions** for profile type).

On Android Enterprise COPE devices, you can configure the **Work profile password** > **Required unlock frequency** setting. Use this setting to select how long users have before they're required to unlock the work profile using a strong authentication method.

For more information on this setting, go to [Android Enterprise device settings to allow or restrict features using Intune](../configuration/device-restrictions-android-for-work.md).

Applies to:
- Android 8.0 and newer
- Android Enterprise corporate owned work profile (COPE)

#### New macOS settings in Settings Catalog<!-- 14158964 -->
The Settings Catalog has new macOS settings you can configure (**Devices** > **Configuration profiles** > **Create profile** > **macOS** for platform >**Settings catalog** for profile type):

**Accounts > Caldav**:

- Cal DAV Account Description
- Cal DAV Host Name
- Cal DAV Password
- Cal DAV Port
- Cal DAV Principal URL
- Cal DAV Use SSL
- Cal DAV Username

**Accounts > Carddav**:

- Card DAV Account Description
- Card DAV Host Name
- Card DAV Password
- Card DAV Port
- Card DAV Principal URL
- Card DAV Use SSL
- Card DAV Username

**User Experience > Dock**:

- Allow Dock Fixup Override
- Auto Hide
- Auto Hide Immutable
- Contents Immutable
- Double Click Behavior
- Double Click Behavior Immutable
- Large Size
- Launch Animation
- Launch Animation Immutable
- Magnification
- Magnification Size Immutable
- Magnify Immutable
- MCX Dock Special Folders
- Minimize Effect
- Minimize Effect Immutable
- Minimize Into Application Immutable
- Minimize To Application
- Orientation
- Persistent Apps
- Persistent Others
- Position Immutable
- Show Indicators Immutable
- Show Process Indicators
- Show Recents
- Show Recents Immutable
- Size Immutable
- Static Apps
- Static Only
- Static Others
- Tile Size
- Window Tabbing
- Window Tabbing Immutable

**System Configuration > Energy Saver**:

- Desktop Power
- Desktop Schedule
- Destroy FV Key On Standby
- Laptop Battery Power
- Laptop Power
- Sleep Disabled

**System Configuration > System Logging**:

- Enable Private Data

**System Configuration > Time Server**:

- Time Server
- Time Zone

The following settings are also in Settings Catalog. Previously, they were only available in Templates:

**Security > Passcode**:

- Allow Simple Passcode
- Change At Next Auth
- Force PIN
- Max Failed Attempts
- Max Grace Period
- Max Inactivity
- Max PIN Age In Days
- Min Complex Characters
- Min Length
- Minutes Until Failed Login Reset
- PIN History
- Require Alphanumeric Passcode

There isn't any conflict resolution between policies created using the Settings catalog and policies created using Templates. When creating new policies in the Settings Catalog, be sure there are no conflicting settings with your current policies.

For more information about configuring Settings catalog profiles in Intune, see [Create a policy using settings catalog in Microsoft Intune](../configuration/settings-catalog.md).

Applies to:
- macOS

#### New Microsoft Office and Microsoft Outlook preference settings in the macOS Settings Catalog<!-- 14193331 -->
The Settings Catalog supports preference settings for Microsoft Office and Microsoft Outlook (**Devices** > **Configuration profiles** > **Create profile** > **macOS** for platform >**Settings catalog** for profile type). 

The following settings are available:

**Microsoft Office > Microsoft Office**:

- Allow experiences and functionality that analyzes user content
- Allow experiences and functionality that downloads user content
- Allow macros to modify Visual Basic projects
- Allow optional connected experiences
- Allow Visual Basic macros to use system APIs
- Background accessibility checking
- Default to local files for open - save
- Diagnostic data level
- Disable cloud fonts
- Disable third-party store add-in catalog
- Disable user surveys
- Enable automatic sign-in
- Prevent all Visual Basic macros from executing
- Prevent Visual Basic macros from using external dynamic libraries
- Prevent Visual Basic macros from using legacy MacScript
- Prevent Visual Basic macros from using pipes to communicate
- Show Template Gallery on app launch
- Show What's New dialog
- Visual Basic macro policy

**Microsoft Office > Microsoft Outlook**:

- Allow S - MIME certificates without a matching email address
- Allowed Email Domains
- Default domain name
- Default weather location
- Disable 'Do Not Forward' options
- Disable automatic updating of weather location
- Disable email signatures
- Disable export to OLM files
- Disable import from OLM and PST files
- Disable Junk settings
- Disable Microsoft 365 encryption options
- Disable Microsoft Teams meeting support
- Disable S - MIME
- Disable Skype for Business meeting support
- Download embedded images
- Enable New Outlook
- Hide On My Computer folders
- Hide the 'Get started with Outlook' control in the task pane
- Hide the 'Personalize the new Outlook' dialog
- Set the order in which S - MIME certificates are considered
- Set theme
- Specify first day of the week
- Trust Office 365 autodiscover redirects
- Use domain-based autodiscover instead of Office 365

For more information about the Settings Catalog, go to:

- [Tasks you can complete using the Settings Catalog in Intune](../configuration/settings-catalog-common-features.md)
- [Create a policy using settings catalog in Microsoft Intune](../configuration/settings-catalog.md)

For more information about Microsoft Office and Outlook settings you can configure, go to:

- [Use preferences to manage privacy controls for Office for Mac - Deploy Office](/deployoffice/privacy/mac-privacy-preferences#preference-setting-for-connected-experiences-that-download-online-content).
- [Set preferences for Outlook for Mac - Deploy Office](/deployoffice/mac/preferences-outlook)

Applies to:
- macOS

### Device management

#### Remotely restart and shut down macOS device<!-- 12472418 -->
You'll be able to remotely restart or shut down a macOS device using device actions. These device actions are available for devices running macOS 10.13 and later. 

For more information, see [Restart devices with Microsoft Intune](../remote-actions/device-restart.md). 

#### Additional Remote actions for Android (AOSP) Corporate devices<!-- 8504019 -->
For Android Open Source Project (AOSP) Corporate devices, you can soon leverage additional remote actions from the Microsoft Endpoint Manager admin center - Reboot and Remote lock. 

For information about these features, see:
 - [Remotely restart devices with Intune](../remote-actions/device-restart.md)
 - [Remotely lock devices with Intune](../remote-actions/device-remote-lock.md).

Applies to:
- Android Open Source Project (AOSP)

#### User configuration support for  Windows 11 multi-session VMs is in public preview<!-- 7231329 -->

You'll be able to:
- Configure user scope policies using **Settings catalog** and assign to groups of users
- Configure user certificates and assign to users
- Configure PowerShell scripts to install in the user context and assign to users

Applies to: 
 - Windows 11

> [!Note]
> User support for Windows 10 multi-session builds will be available later this year.

For more information, go to
[Using Azure Virtual Desktop multi-session with Microsoft Intune](../fundamentals/azure-virtual-desktop-multi-session.md)

#### View a managed device's group membership<!-- 4100067 -->
In the monitor section of the **Devices** workload of Intune, you can view the group membership of all Azure AD groups for a managed device. You can select **Group Membership** by signing in to [Microsoft Endpoint Manager admin center](https://go.microsoft.com/fwlink/?linkid=2109431) and selecting **Devices** > **All devices** > *select a device* > **Group Membership**. For more information, see [Device group membership report](../fundamentals/reports.md#device-group-membership-report-organizational).

#### Improved certificate reporting details<!-- 13316515 -->
We’ve changed what Intune displays when you view certificate details for devices and certificate profiles. To view the report, in the [Microsoft Endpoint Manager admin center](https://go.microsoft.com/fwlink/?linkid=2109431) go to > **Devices** > **Monitor** > **Certificates**.

With the improved reporting view, Intune displays information for the following:

- Valid certificates
- Certificates that were revoked within the last 30 days
- Certificates that expired within the last 30 days

The report no longer displays details for certificates that are not valid or that are no longer on a device.

### Device enrollment

### Utilize bootstrap tokens on macOS devices<!-- 12693392 -->
Bootstrap token support, previously in public preview, is now generally available to all Microsoft Intune customers, including GCC High and Microsoft Azure Government Cloud tenants. Intune supports the use of bootstrap tokens on enrolled devices running macOS, version 10.15 or later.

Bootstrap tokens allow for non-admin users to have increased MDM permissions, and perform specific software functions on behalf of the IT admin.  Bootstrap tokens is supported on:  

- Supervised devices (in Intune, that's all user-approved enrollments)  
- Devices enrolled in Intune via Apple automated device enrollment   

For more information about how bootstrap tokens work with Intune, see [Set up enrollment for macOS devices](../enrollment/macos-enroll.md#bootstrap-tokens).

### Intune apps

#### Newly available protected apps for Intune<!-- 14469921, 14645753 -->
The following protected apps are now available for Microsoft Intune:

- Condeco by Condeco Limited
- RICOH Spaces by Ricoh Digital Services

For more information about protected apps, see [Microsoft Intune protected apps](../apps/apps-supported-intune-apps.md).

## What's new archive

For previous months, see the [What's new archive](whats-new-archive.md).

## Notices

[!INCLUDE [Intune notices](../includes/intune-notices.md)]
