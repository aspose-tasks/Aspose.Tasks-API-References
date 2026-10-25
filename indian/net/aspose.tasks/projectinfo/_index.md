---
title: "क्लास ProjectInfo"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.ProjectInfo क्लास। Project Online पर उपलब्ध प्रकाशित प्रोजेक्ट के बारे में संक्षिप्त जानकारी।"
type: docs
weight: 1470
url: /hi/net/aspose.tasks/projectinfo/
---
## ProjectInfo class

Project Online पर उपलब्ध प्रकाशित प्रोजेक्ट के बारे में संक्षिप्त जानकारी।

```csharp
public sealed class ProjectInfo
```

## कन्स्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [ProjectInfo](projectinfo/)() | `ProjectInfo` क्लास की नई इंस्टेंस को इनिशियलाइज़ करता है। |

## गुण

| नाम | विवरण |
| --- | --- |
| [CreatedDate](../../aspose.tasks/projectinfo/createddate/) { get; } | प्रोजेक्ट के निर्मित होने की तिथि और समय प्राप्त करता है। |
| [Description](../../aspose.tasks/projectinfo/description/) { get; } | प्रोजेक्ट का विवरण प्राप्त करता है। |
| [Id](../../aspose.tasks/projectinfo/id/) { get; } | प्रोजेक्ट का अद्वितीय पहचानकर्ता प्राप्त करता है। |
| [IsCheckedOut](../../aspose.tasks/projectinfo/ischeckedout/) { get; } | एक मान प्राप्त करता है जो दर्शाता है कि प्रोजेक्ट चेक आउट है या नहीं। |
| [LastPublishedDate](../../aspose.tasks/projectinfo/lastpublisheddate/) { get; } | प्रोजेक्ट के प्रकाशित होने की सबसे हालिया तिथि प्राप्त करता है। |
| [LastSavedDate](../../aspose.tasks/projectinfo/lastsaveddate/) { get; } | प्रोजेक्ट के सहेजे जाने की सबसे हालिया तिथि प्राप्त करता है। |
| [Name](../../aspose.tasks/projectinfo/name/) { get; } | प्रोजेक्ट का नाम प्राप्त करता है। |

## उदाहरण

दिखाता है कि Project Online से प्रोजेक्ट्स की जानकारी कैसे पढ़ी जाए।

```csharp
const string SharepointDomainAddress = "https://contoso.sharepoint.com/sites/pwa";
const string UserName = "admin@contoso.onmicrosoft.com";
const string Password = "MyPassword";

var credentials = new ProjectServerCredentials(SharepointDomainAddress, UserName, Password);

var reader = new ProjectServerManager(credentials);
IEnumerable<ProjectInfo> list = reader.GetProjectList();

// प्रोजेक्ट की जानकारी पढ़ें
Console.WriteLine("Print information about projects:");
foreach (var info in list)
{
    Console.WriteLine("Id: " + info.Id);
    Console.WriteLine("Name: " + info.Name);
    Console.WriteLine("Description: " + info.Description);
    Console.WriteLine("Created Date: " + info.CreatedDate);
    Console.WriteLine("Last Saved Date: " + info.LastSavedDate);
    Console.WriteLine("Last Published Date: " + info.LastPublishedDate);
    Console.WriteLine("Is Checked Out: " + info.IsCheckedOut);
}
```

### संबंधित देखें

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


