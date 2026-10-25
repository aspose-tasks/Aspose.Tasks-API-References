---
title: "ProjectServerManager.GetProjectList"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "ProjectServerManager मेथड। वर्तमान Project Online खाते / Project Server इंस्टेंस के वर्किंग स्टोर से प्रोजेक्ट्स की सूची प्राप्त करता है।"
type: docs
weight: 50
url: /hi/net/aspose.tasks/projectservermanager/getprojectlist/
---
## ProjectServerManager.GetProjectList method

वर्तमान Project Online खाते \\ Project Server इंस्टेंस के 'Working' स्टोर से प्रोजेक्ट्स की सूची प्राप्त करता है।

```csharp
public IEnumerable<ProjectInfo> GetProjectList()
```

### रिटर्न वैल्यू

वर्तमान Project Online खाते \\ Project Server इंस्टेंस में प्रोजेक्ट्स की सूची।

## उदाहरण

Microsoft Project Online से प्रोजेक्ट पढ़ने का तरीका दिखाता है।

```csharp
const string SharepointDomainAddress = "https://contoso.sharepoint.com/sites/pwa";
const string UserName = "admin@contoso.onmicrosoft.com";
const string Password = "MyPassword";

var credentials = new ProjectServerCredentials(SharepointDomainAddress, UserName, Password);
var manager = new ProjectServerManager(credentials);
IEnumerable<ProjectInfo> list = manager.GetProjectList();

foreach (var info in list)
{
    var project = manager.GetProject(info.Id);
    Console.WriteLine("{0} - {1} - {2}", info.Name, info.CreatedDate, info.LastSavedDate);
    Console.WriteLine("Resources count: {0}", project.Resources.Count);
}
```

### संबंधित देखें

* class [ProjectInfo](../../projectinfo/)
* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)


