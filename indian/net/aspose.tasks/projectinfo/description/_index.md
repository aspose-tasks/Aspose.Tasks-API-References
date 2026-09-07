---
title: "ProjectInfo.Description"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "ProjectInfo प्रॉपर्टी। प्रोजेक्ट का विवरण प्राप्त करता है।"
type: docs
weight: 30
url: /hi/net/aspose.tasks/projectinfo/description/
---
## ProjectInfo.Description property

प्रोजेक्ट का विवरण प्राप्त करता है।

```csharp
public string Description { get; }
```

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

* class [ProjectInfo](../)
* namespace [Aspose.Tasks](../../projectinfo/)
* assembly [Aspose.Tasks](../../../)


