---
title: "क्लास ProjectServerSaveOptions"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.ProjectServerSaveOptions क्लास। प्रोजेक्ट को Project Server या Project Online पर सहेजते समय अतिरिक्त विकल्प निर्दिष्ट करने की अनुमति देता है।"
type: docs
weight: 1510
url: /hi/net/aspose.tasks/projectserversaveoptions/
---
## ProjectServerSaveOptions class

जब प्रोजेक्ट को प्रोजेक्ट सर्वर या प्रोजेक्ट ऑनलाइन में सहेजा जाता है तो अतिरिक्त विकल्प निर्दिष्ट करने की अनुमति देता है।

```csharp
public sealed class ProjectServerSaveOptions
```

## कन्स्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [ProjectServerSaveOptions](projectserversaveoptions/)() | `ProjectServerSaveOptions` वर्ग का नया उदाहरण आरंभ करता है। |

## गुण

| नाम | विवरण |
| --- | --- |
| [PollingInterval](../../aspose.tasks/projectserversaveoptions/pollinginterval/) { get; set; } | क्यू जॉब स्थिति अनुरोधों के बीच अंतराल प्राप्त करता है या सेट करता है। डिफ़ॉल्ट मान 2 सेकंड है। |
| [ProjectGuid](../../aspose.tasks/projectserversaveoptions/projectguid/) { get; set; } | प्रोजेक्ट का अद्वितीय पहचानकर्ता प्राप्त करता है या सेट करता है। यह Project Server \\ Project Online उदाहरण के भीतर अद्वितीय होना चाहिए। |
| [ProjectName](../../aspose.tasks/projectserversaveoptions/projectname/) { get; set; } | Project Server \\ Project Online प्रोजेक्ट सूची में प्रदर्शित होने वाले प्रोजेक्ट का नाम प्राप्त करता है या सेट करता है। यह Project Server \\ Project Online उदाहरण के भीतर अद्वितीय होना चाहिए। यदि मान छोड़ा जाता है, तो Prj.Name प्रॉपर्टी का मान उपयोग किया जाएगा। |
| [Timeout](../../aspose.tasks/projectserversaveoptions/timeout/) { get; set; } | Project Server की क्यू प्रोसेसिंग सेवा द्वारा प्रोजेक्ट सहेजने के अनुरोध की प्रोसेसिंग की प्रतीक्षा करते समय उपयोग किए जाने वाले टाइमआउट को प्राप्त करता है या सेट करता है। इस प्रॉपर्टी का डिफ़ॉल्ट मान 1 मिनट है। |

## उदाहरण

ऑन-प्रेमाइस Project Server उदाहरण में नया प्रोजेक्ट बनाने के लिए &lt;see cref=\"Aspose.Tasks.ProjectServerSaveOptions\" /&gt; विकल्पों का उपयोग कैसे करें, दिखाता है।

```csharp
try
{
    const string URL = "https://project_server.local/sites/pwa";
    const string Domain = "CONTOSO.COM";
    const string UserName = "Administrator";
    const string Password = "MyPassword";

    var project = new Project(DataDir + @"Project1.mpp");

    var windowsCredentials = new NetworkCredential(UserName, Password, Domain);
    var projectServerCredentials = new ProjectServerCredentials(URL, windowsCredentials);
    var manager = new ProjectServerManager(projectServerCredentials);
    var options = new ProjectServerSaveOptions
                      {
                          ProjectGuid = Guid.NewGuid(),
                          ProjectName = "New project",
                          Timeout = TimeSpan.FromMinutes(5),
                          PollingInterval = TimeSpan.FromSeconds(3)
                      };

    manager.CreateNewProject(project, options);
}
catch (ProjectOnlineException ex)
{
    Console.WriteLine(ex.Message);
}
```

### संबंधित देखें

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


