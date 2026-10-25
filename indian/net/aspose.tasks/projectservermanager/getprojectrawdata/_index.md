---
title: "ProjectServerManager.GetProjectRawData"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "ProjectServerManager मेथड। समस्या निवारण के उद्देश्य से प्रोजेक्ट का बाइनरी डेटा प्राप्त करता है।"
type: docs
weight: 60
url: /hi/net/aspose.tasks/projectservermanager/getprojectrawdata/
---
## ProjectServerManager.GetProjectRawData method

समस्या निवारण के लिए प्रोजेक्ट का बाइनरी डेटा प्राप्त करता है।

```csharp
public Stream GetProjectRawData(Guid projectGuid)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| projectGuid | Guid | पढ़ने के लिए प्रोजेक्ट का Guid। |

### रिटर्न वैल्यू

कच्चे प्रोजेक्ट डेटा वाली स्ट्रीम।

## उदाहरण

```csharp
In this example the debug info for the specific project is retrieved. You can pass the resulting "debug.zip" to the support team for troubleshooting purposes.
[C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "password");
// जिस प्रोजेक्ट को आप प्राप्त करना चाहते हैं उसका GUID।
var projectGuid = new Guid("e0294bfb-5657-45c8-9cc5-82169fb95d69");
ProjectServerManager manager = new ProjectServerManager(credentials);
using (var fileStream = File.OpenWrite(@"c:\debug.zip"))
{
    using (var stream = manager.GetProjectRawData(projectGuid))
    {
        stream.CopyTo(fileStream);
    }
}
```

समस्या निवारण के लिए Microsoft Project Online से प्रोजेक्ट का कच्चा डेटा प्राप्त करने का तरीका दर्शाता है।

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

    // उपयोगकर्ता समस्या निवारण के लिए प्रोजेक्ट को कच्ची डेटा स्ट्रीम के रूप में पढ़ सकता है।
    using (FileStream fs = File.Create(OutDir + "projectRawData.zip"))
    {
        using (var stream = manager.GetProjectRawData(info.Id))
        {
            stream.CopyTo(fs);
        }
    }

    // आप परिणामस्वरूप फ़ाइल को सपोर्ट को भेज सकते हैं।
}
```

### संबंधित देखें

* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)


