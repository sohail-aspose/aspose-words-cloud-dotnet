# Aspose.Words Cloud SDK for .NET [![NuGet](https://img.shields.io/nuget/v/Aspose.Words-Cloud.svg)](https://www.nuget.org/packages/Aspose.Words-Cloud/)
This repository contains Aspose.Words Cloud SDK for .NET source code. This SDK allows you to work with Aspose.Words Cloud REST APIs in your .NET applications quickly and easily, with zero initial cost.

# Key Features
* Conversion between various document-related formats (20+ formats supported), including PDF<->Word conversion
* Mail merge and reports generation 
* Splitting Word documents
* Accessing Word document metadata and statistics
* Find and replace
* Watermarks and protection
* Full read & write access to Document Object Model, including sections, paragraphs, text, images, tables, headers/footers and many others

See [API Reference](https://apireference.aspose.cloud/words/) for full API specification.

## How to use the SDK?
The complete source code is available in this repository folder. You can either directly use it in your project via source code or get [NuGet distribution](https://www.nuget.org/packages/Aspose.Words-Cloud/) (recommended). For more details, please visit our [documentation website](https://docs.aspose.cloud/display/wordscloud/Available+SDKs#AvailableSDKs-.NET).

### Prerequisites

To use Aspose Words for Cloud .NET SDK you need to register an account with [Aspose Cloud](https://www.aspose.cloud/) and lookup/create App Key and SID at [Cloud Dashboard](https://dashboard.aspose.cloud/#/apps). There is free quota available. For more details, see [Aspose Cloud Pricing](https://purchase.aspose.cloud/pricing).

### Installation

#### Install Aspose.Words-Cloud via NuGet

From the command line:

	nuget install Aspose.Words-Cloud

From Package Manager:

	PM> Install-Package Aspose.Words-Cloud

From within Visual Studio:

1. Open the Solution Explorer.
2. Right-click on a project within your solution.
3. Click on *Manage NuGet Packages...*
4. Click on the *Browse* tab and search for "Aspose.Words-Cloud".
5. Click on the Aspose.Words-Cloud package, select the appropriate version in the right-tab and click *Install*.

### Sample usage

The examples below show how your application have to initiate and convert "doc" file to "pdf" using Aspose.Words-Cloud library:
```csharp
var wordsApi = new WordsApi(AppKey, AppSid);
var saveOptionsData = new SaveOptionsData { SaveFormat = "pdf", FileName = "destination.pdf" };
var request = new PostDocumentSaveAsRequest("fileStoredInCloud.doc", saveOptionsData);            
wordsApi.PostDocumentSaveAs(request);
```

[Tests](Aspose.Words.Cloud.Sdk.Tests) contain various examples of using the SDK.

## Dependencies
- .NET Framework 2.0 or later
- [Json.NET](https://www.nuget.org/packages/Newtonsoft.Json/)

## Comparison with Old generation SDK
New SDK has the following advantages over the [previous version](https://github.com/aspose-words/Aspose.Words-for-Cloud):
+ SDK is fully in sync with the API, all missing methods are added
+ Classes, methods and properties have comments and are IDE-friendly
+ Better security
+ Usage of Request/Response classes to represent long lists of parameters. This allows for cleaner code and easier backwards-compatibility going forward

New SDK is not backwards compatible with previous generation because of the last item. It should be straightforward to convert your code to using Request/Response objects, if you need any help on migration please ask at [Free Support Forums](https://forum.aspose.cloud/c/words).

## Contact Us
Your feedback is very important to us. Please feel free to contact us using our [Support Forums](https://forum.aspose.cloud/c/words).
