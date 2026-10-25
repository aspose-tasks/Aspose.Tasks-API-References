---
title: "ProjectServerManager.GetProject"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "ProjectServerManager मेथड। निर्दिष्ट guid वाले प्रोजेक्ट को Project Online खाते के Project Server इंस्टेंस से प्राप्त करता है"
type: docs
weight: 40
url: /hi/net/aspose.tasks/projectservermanager/getproject/
---
## ProjectServerManager.GetProject method

निर्दिष्ट GUID के साथ प्रोजेक्ट को Project Online खाते \\ Project Server इंस्टेंस से प्राप्त करता है।

```csharp
public Project GetProject(Guid projectGuid)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| projectGuid | Guid | पढ़ने के लिए प्रोजेक्ट का Guid। |

### रिटर्न वैल्यू

`[`Project`](../../project/)` क्लास का इंस्टेंस जो Project Online \ Project Server से पढ़े गए प्रोजेक्ट का प्रतिनिधित्व करता है।

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

* class [Project](../../project/)
* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)


