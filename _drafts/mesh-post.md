# Unpacking Microsoft Mesh

## Introduction

Hello everyone. At Microsoft Ignite, the Microsoft team provided significant information about Microsoft Mesh, a Mixed Reality platform that aims to power immersive applications that allow users to collaborate from a multitude of devices, including virtual reality headsets, desktops, and mobile devices. As a developer using the Microsoft platform who has some experience building simulations with the Unity game engine, I wanted to learn more about what Mesh has to offer.

## The Tenets of Mesh

Before discussing the features that Mesh offers for developers, we need to establish some fundamental concepts. In a [demo shown on Microsoft Mechanics](https://www.youtube.com/watch?v=lhKn9mjy_QM), Simon Skaria mentions that experiences in Microsoft Mesh are built around *spaces*. Spaces implement the four core areas that Mesh aims to revolutionize. 

The first tenet of Microsoft Mesh is *presence*. Presence provides offerings in the spectrum between realism and reach. Basically, it allows users to represent themselves in the immersive environment through holoportation or as avatars (which the user can provide). Look at this image from the [Microsoft Ignite session about Mesh](https://www.youtube.com/watch?v=HZkL-A2i_LM).

![](./mesh-post/individual-representation.png)

Second, Microsoft explains that Mesh can be used to enhance environments with holographic presentations, like enhancing a view of a city with holographic markers. *Spatial maps* enable this by aligning visual enhancements with physical objects and allow users of multiple devices to see these markings.

Third, Mesh provides *holographic rendering*. In the Ignite session, Skaria demonstrates how drone images of a bridge can be reconstructed to enable inspectors to verify its integrity. Rendering takes place on the Edge or in the cloud. This flexibility allows users to collaborate on high-poly 3D models without being impacted by the compute capabilities of their hardware. For industrial customers, Mesh’s rendering capabilities are compatible with a variety of industry formats spanning software made by Autodesk, Siemens, Dassault Systems, and more. 

![](./mesh-post/rendering-bridge.png)

Lastly, Microsoft has implemented *multi-user sync*, which enables users across different platforms to observe user actions within 100ms latency, irrespective of their geographic location. The image below is particularly fascinating because it shows how users of native 2D and 3D devices can engage over the Mesh platform. Multi-user sync also supports spatial audio to further enhance immersion.

![](./mesh-post/multiuser-sync.png)

## How can developers get started?

Microsoft Mesh offers to solve the fundamental problems of Mixed Reality that prevent businesses from adopting MR solutions. However, the Mesh ecosystem needs to be accessible to developers. Luckily, I believe that Microsoft is poised to help developers deliver on the promise of MR.

First off, Mesh is based on the Azure platform. This means that Microsoft's identity solutions, including Azure Active Directory, support MR applications that meet corporate security standards. Compatibility with Microsoft Graph means [integration with Microsoft 365 and the insights it offers.](https://developer.microsoft.com/en-us/microsoft-365/blogs/microsoft-graph-mailbag-intro-to-microsoft-graph-and-top-5-api-requests/)

During the Microsoft Ignite session, Dorrene Brown shows how to build a Microsoft Mesh-enabled application using the Unity SDK. In summary, here's the steps followed:

1. Enable Mesh-based applications in the Azure Active Directory tenant and allow them to use Microsoft Graph APIs and Mixed Reality services

2. Add the Microsoft Mesh SDK to your Unity application and use the included Unity prefabs in your app

3. Use the included Unity tooling, including the Microsoft Mesh editor window, to authenticate the application with Azure and manage Mesh sessions

4. Import a 3D model from OneDrive to render in the environment

While these steps seem simple, it doesn't look like the Unity SDK is publicly available yet. However, I will update this post when it is.

## Conclusion

Today, I've just given a high-level overview of Mesh. I look forward to building some basic applications using Microsoft Mesh as the service becomes available. For now, I would recommend [subscribing to Microsoft Mesh updates.](https://info.microsoft.com/CO-NOGEP-CNTNT-FY21-03Mar-02-Microsoft-Mesh-5890_01Registration-ForminBody.html) In addition, the [Mesh documentation](https://docs.microsoft.com/en-us/mesh/) provide a good starting point, though there's little information on the client SDKs.