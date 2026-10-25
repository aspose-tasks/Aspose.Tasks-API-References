---
title: "क्लास ProjectServerCredentials"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.ProjectServerCredentials क्लास। क्रेडेंशियल्स जो Project Online या ऑन-प्रिमाइसेस Project Server इंस्टेंस से कनेक्ट करने के लिए उपयोग होते हैं।"
type: docs
weight: 1490
url: /hi/net/aspose.tasks/projectservercredentials/
---
## ProjectServerCredentials class

प्रोजेक्ट ऑनलाइन या प्रोजेक्ट सर्वर के ऑन-प्रेमाइस इंस्टेंस से कनेक्ट होने के लिए उपयोग किए जाने वाले क्रेडेंशियल्स।

```csharp
public sealed class ProjectServerCredentials
```

## कन्स्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [ProjectServerCredentials](projectservercredentials/#constructor)(string, NetworkCredential) | `ProjectServerCredentials` क्लास का नया इंस्टेंस प्रारंभ करता है, जिसमें Project Web Access एंडपॉइंट का URL और नेटवर्क क्रेडेंशियल्स उपयोग किए जाते हैं। |
| [ProjectServerCredentials](projectservercredentials/#constructor_1)(string, string) | `ProjectServerCredentials` क्लास का नया इंस्टेंस प्रारंभ करता है, जिसमें SharePoint साइट का URL और SharePoint के PWA (Project Web Access) साइट के लिए वैध SPOIDCRL प्राधिकरण टोकन उपयोग किया जाता है। |
| [ProjectServerCredentials](projectservercredentials/#constructor_2)(string, string, string) | `ProjectServerCredentials` क्लास का नया इंस्टेंस प्रारंभ करता है, जिसमें SharePoint साइट का URL, उपयोगकर्ता नाम और पासवर्ड उपयोग किए जाते हैं। |

## गुण

| नाम | विवरण |
| --- | --- |
| [AuthToken](../../aspose.tasks/projectservercredentials/authtoken/) { get; } | SharePoint इंस्टेंस के लिए प्राधिकरण टोकन प्राप्त करता है। |
| [SiteUrl](../../aspose.tasks/projectservercredentials/siteurl/) { get; } | SharePoint साइट पर PWA का URL या ऑन-प्रिमाइसेस Project Server का URL प्राप्त करता है। उदाहरण के लिए, https://your_company_name.sharepoint.com/sites/pwa\"; |
| [UserName](../../aspose.tasks/projectservercredentials/username/) { get; } | SharePoint साइट के लिए उपयोगकर्ता नाम प्राप्त करता है। |

## विधियाँ

| नाम | विवरण |
| --- | --- |
| override [ToString](../../aspose.tasks/projectservercredentials/tostring/)() | इस इंस्टेंस का स्ट्रिंग प्रतिनिधित्व लौटाता है। |

## उदाहरण

विवरण देता है कि Microsoft Project Online से प्रोजेक्ट की सूची प्राप्त करने के लिए प्रोजेक्ट सर्वर क्रेडेंशियल्स का उपयोग कैसे करें।

```csharp
try
{
    const string SharepointDomainAddress = "https://contoso.sharepoint.com/sites/pwa";
    const string UserName = "admin@contoso.onmicrosoft.com";
    const string Password = "MyPassword";

    var credentials = new ProjectServerCredentials(SharepointDomainAddress, UserName, Password);

    var newProject = new Project(DataDir + @"Project1.mpp");

    var manager = new ProjectServerManager(credentials);
    manager.CreateNewProject(newProject);

    IEnumerable<ProjectInfo> list = manager.GetProjectList();

    foreach (var info in list)
    {
        var project = manager.GetProject(info.Id);
        Console.WriteLine("{0} - {1} - {2}", info.Name, info.CreatedDate, info.LastSavedDate);
        Console.WriteLine("Resources count: {0}", project.Resources.Count);
    }
}
catch (ProjectOnlineException ex)
{
    Console.WriteLine(ex.Message);
}
```

### संबंधित देखें

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


