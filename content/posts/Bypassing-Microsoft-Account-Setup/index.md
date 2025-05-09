---
title: "Bypassing Microsoft Account Setup in Windows 11 Using start ms-cxh:localonly: A Comprehensive Guide"
date: 2022-06-25
description: "Understanding the `start ms-cxh:localonly` Command in Windows 11"
tags: ["Windows"]
---


# Understanding the `start ms-cxh:localonly` Command in Windows 11

## Introduction

Windows 11 has introduced several changes to the user experience, including a stronger emphasis on integrating Microsoft accounts during the setup process. However, for users and administrators who prefer or require local accounts, the `start ms-cxh:localonly` command offers a valuable workaround. This article delves into the technical aspects of this command, its usage, and its broader implications.

## What Is `start ms-cxh:localonly`?

The `start ms-cxh:localonly` command is a URI (Uniform Resource Identifier) scheme used within Windows 11 to initiate the local account creation process during the Out-of-Box Experience (OOBE). By executing this command, users can bypass the default requirement to sign in with or create a Microsoft account during setup.

### Breakdown of the Command

- **`start`**: A command-line instruction used to initiate a program or process.
- **`ms-cxh:localonly`**: A URI scheme that triggers the local account setup interface within the Windows 11 OOBE.

This command effectively redirects the setup process from the cloud-based Microsoft account creation to a local account setup, providing users with an alternative path during installation.

## Historical Context

In earlier versions of Windows, users had the option to create local accounts during setup without significant hurdles. However, Windows 11 has shifted towards a cloud-centric approach, often requiring users to sign in with a Microsoft account. While this integration offers benefits like seamless synchronization and access to Microsoft services, it has raised concerns among users who prefer local accounts for privacy, security, or organizational policies.

Previously, users employed the `oobe\bypassnro` command to circumvent the Microsoft account requirement. However, Microsoft has removed this method in recent builds, prompting the need for alternative solutions like `start ms-cxh:localonly`.

## Practical Applications

### Bypassing Microsoft Account Requirement

During the Windows 11 setup process, users can invoke the `start ms-cxh:localonly` command to bypass the Microsoft account requirement. This is particularly useful in scenarios where internet access is unavailable or when users prefer not to associate their device with a Microsoft account.

### Enterprise and Organizational Use

Organizations often have policies that mandate the use of local accounts for security and compliance reasons. By utilizing this command, IT administrators can streamline the deployment of Windows 11 across multiple devices without the need to configure Microsoft accounts for each user.

### Privacy-Conscious Users

For individuals concerned about data privacy, creating a local account ensures that personal information is not automatically synced with Microsoft's cloud services. This approach minimizes data exposure and provides greater control over personal information.

## Step-by-Step Guide to Using `start ms-cxh:localonly`

1. **Initiate Windows 11 Setup**: Begin the installation process as usual.
2. **Access Command Prompt**: When prompted to sign in with a Microsoft account, press `Shift + F10` to open the Command Prompt.
3. **Execute the Command**: Type `start ms-cxh:localonly` and press `Enter`.
4. **Create Local Account**: A window will appear, allowing you to create a local user account by entering a username and password.
5. **Continue Setup**: Proceed with the remaining setup steps, such as configuring privacy settings.

This method is straightforward and does not require disconnecting from the internet or modifying system files.

## Technical Considerations

### URI Schemes in Windows

Windows utilizes URI schemes to facilitate communication between applications and system components. The `ms-cxh` scheme is associated with the Cloud Experience Host, which manages the OOBE process. By appending `localonly`, the command instructs the system to initiate the local account setup interface instead of the default Microsoft account creation.

### Compatibility

The `start ms-cxh:localonly` command is compatible with various editions of Windows 11, including Home and Pro. However, its functionality may be subject to change in future updates, as Microsoft continues to refine the setup experience. Users should verify compatibility with their specific Windows 11 build before relying on this method.

## Security and Privacy Implications

### Data Sovereignty

Creating a local account ensures that user data remains stored locally on the device, aligning with data sovereignty requirements in certain jurisdictions. This approach is beneficial for organizations operating under strict data protection regulations.

### Reduced Attack Surface

By avoiding the integration of a Microsoft account, users can minimize the attack surface associated with cloud-based services. This reduces the risk of unauthorized access to personal data through compromised Microsoft accounts.

### Compliance with Organizational Policies

Many organizations have policies that restrict the use of external accounts or cloud services. Utilizing local accounts during setup ensures compliance with such policies and simplifies device management within the organization.

## Limitations and Considerations

### Feature Restrictions

Users who opt for local accounts may not have immediate access to certain features that require a Microsoft account, such as OneDrive integration, Microsoft Store access, and synchronization of settings across devices. However, these features can be enabled later by signing in with a Microsoft account if desired.

### Potential Deprecation

As Microsoft continues to evolve the Windows operating system, there is a possibility that methods like `start ms-cxh:localonly` may be deprecated in future updates. Users and administrators should stay informed about changes to the setup process and be prepared to adapt their deployment strategies accordingly.

## Conclusion

The `start ms-cxh:localonly` command serves as a valuable tool for users and organizations seeking to create local accounts during the Windows 11 setup process. By understanding its functionality and implications, users can make informed decisions that align with their privacy preferences and organizational requirements. While this method provides a convenient workaround, it is essential to remain vigilant about potential changes in future Windows updates that may affect its availability.

## Sources

- [Windows Central](https://www.windowscentral.com/software-apps/windows-11/an-even-better-microsoft-account-bypass-for-windows-11-has-already-been-discovered)
- [Bleeping Computer](https://www.bleepingcomputer.com/news/microsoft/new-windows-11-trick-lets-you-bypass-microsoft-account-requirement/)
- [Pureinfotech](https://pureinfotech.com/bypass-microsoft-account-setup-windows-11/)
- [Wintips.org](https://www.wintips.org/how-to-install-windows-11-with-local-account-april-2025/)
