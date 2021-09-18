# WorldServer documentation for software developers #
In WorldServer, software developers can enhance standard functionality through the Software Development Kit (SDK), manage integrations via web services, or customize the user interface by adding new buttons, messages, or other elements.
## Working with the Software Development Kit (SDK) ##
The Software Development Kit (SDK) provides a stable, clearly defined layer of APIs for enhancing standard WorldServer features and for integrating WorldServer with other custom or third-party applications.
### [About the WorldServer SDK](https://docs.rws.com/860026/488074/worldserver-11-7-developer-documentation/about-the-worldserver-sdk) ###
By using the WorldServer SDK, you can implement and manage your own extensions in-house. In other words, you can have complete control over WorldServer customizations.
### [About installing the WorldServer SDK](https://docs.rws.com/860026/501267/worldserver-11-7-developer-documentation/about-installing-the-worldserver-sdk) ###
You can find the SDK installation archive in the WorldServer distribution kit. The archive contains the following: the libraries that you need to create and compile SDK applications, Java documentation for the SDK, additional documentation, and sample code that illustrates how to create WorldServer SDK applications.
### [SDK samples](https://docs.rws.com/860026/501271/worldserver-11-7-developer-documentation/sdk-samples) ###
You can use the sample tools and components included in the samples directory to find out how to make the most of the WorldServer SDK.
### [SDK services and features](https://docs.rws.com/860026/488138/worldserver-11-7-developer-documentation/sdk-services-and-features) ###
The following services are supported primarily through the APIs of the WorldServer SDK. Many of them, however, are also exposed through web services. You can also create custom web services in the SDK, which gives you great flexibility in integrating with WorldServer.
### [Architecture overview](https://docs.rws.com/860026/488086/worldserver-11-7-developer-documentation/architecture-overview) ###
An overview of the WorldServer environment, components, objects, modules, and services that you can access with the SDK.
### [Creating and deploying custom access modules](https://docs.rws.com/860026/488130/worldserver-11-7-developer-documentation/creating-and-deploying-custom-access-modules) ###
Custom access modules are programs or components that have been developed by using the WorldServer SDK. You can create two types of custom access modules: external service modules and component modules.
### [Components supported by the WorldServer SDK](https://docs.rws.com/860026/488157/worldserver-11-7-developer-documentation/components-supported-by-the-worldserver-sdk) ###
A brief description of the components supported by the SDK. Most of the content that might be relevant for developers is provided in the package and object-level Java documentation. The SDK also includes documented samples for each supported component.
### [Other objects that you can configure](https://docs.rws.com/860026/488245/worldserver-11-7-developer-documentation/other-objects-that-you-can-configure) ###
You can configure several types of non-component objects both through the WorldServer user interface and externally, through the components archive.
### [Resources for web services](https://docs.rws.com/860026/859627/worldserver-11-7-developer-documentation/resources-for-web-services) ###
An overview of the SDK components that make up the web service resources.
### [Sample tools and components for customizing web services](https://docs.rws.com/860026/859635/worldserver-11-7-developer-documentation/sample-tools-and-components-for-customizing-web-services) ###
An overview of the sample tools and components that provide models for customizing web services.
## The WorldServer REST API ##
As of version 11.0, WorldServer contains an API based on modern standards (REST and JSON), implemented using the Spring Framework. It uses standard HTTP methods such as GET, POST, PATCH, or DELETE and provides a new layer of security to the WorldServer 11 interface, which is built on top of it.
### [API release notes](https://docs.rws.com/860026/708306/worldserver-11-7-developer-documentation/api-release-notes) ###
An overview of the main changes made to the REST API in WorldServer 11.7.
### [Overview and common flows](https://docs.rws.com/860026/481814/worldserver-11-7-developer-documentation/overview-and-common-flows) ###
Some operations that use the WorldServer API are more complex than others. Before you make a request, you might need to obtain certain information through other requests. For example, before you can complete a task step, you need to find out the ID of the transition to the next step. The topics in this section present the requests you need to make and the order in which you need to make them to perform a series of common operations with the WorldServer API.
### [REST API endpoints](https://docs.rws.com/860026/488286/worldserver-11-7-developer-documentation/rest-api-endpoints) ###
Find out what endpoints you can call and what methods you can use to call each endpoint. You can also find sample calls, potential error messages, and a response for each call.
### [Customizing the REST API](https://docs.rws.com/860026/814420/worldserver-11-7-developer-documentation/customizing-the-rest-api) ###
Add custom endpoints to the new REST API by using the existing WorldServer SDK. However, you should use this only as an entry point into the REST API and delegate the customization logic to other classes.
## Customizations for the WorldServer user interface ##
By using the customization SDK, you can develop user interface elements for various scenarios, such as adding a button on the ribbon, having a dialog box displayed, or customizing a task completion screen.
From a technical standpoint, you can add a customization anywhere on the WorldServer user interface. However, doing so without a customization SDK would be difficult and not recommended. As time passes by and the user interface changes, the customization SDK helps you to manage your own customizations and to maintain a certain level of consistency with the standard WorldServer interface.
**Note:** The customization SDK refers to a set of options that you have when customizing the interface. It has no representation within the actual SDK in the WorldServer distribution kit.
### [Available controls](https://docs.rws.com/860026/489240/worldserver-11-7-developer-documentation/available-controls) ###
The customization SDK contains several UI controls that you can inject as require dependencies. These controls are located in the *sdk/controls/<control-name>* namespace.
### [Available services](https://docs.rws.com/860026/501848/worldserver-11-7-developer-documentation/available-services) ###
The customization SDK contains several UI services that you can inject as require dependencies. These services are located in the *sdk/services* namespace.
### [Sample UI customizations](https://docs.rws.com/860026/865367/worldserver-11-7-developer-documentation/sample-ui-customizations) ###
Links to sample UI customizations that you can download, add to a test environment, and use as starting points for your own customizations.
### [Working with UI customizations](https://docs.rws.com/860026/481770/worldserver-11-7-developer-documentation/working-with-ui-customizations) ###
Starting with version 11.1, you can implement and manage UI customizations directly from WorldServer by logging in as an administrator and typing the following in your browser's address bar: *<ws-host>:<ws-port>/ws/customizations*, where *<ws-host>* is the name or IP address of the machine on which WorldServer is installed and *<ws-port>* is the number of the port on which WorldServer is installed.
