---
title: "क्लास ProjectServerManager"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.ProjectServerManager क्लास। यह क्लास निर्दिष्ट Project Online खाते या निर्दिष्ट ऑन‑प्रेमाइज़ Project Server इंस्टेंस में प्रोजेक्ट्स को पढ़ने और संचालन करने के लिए मेथड्स प्रदान करती है। Project Server के संस्करण 2016 और 2019 समर्थित हैं।"
type: docs
weight: 1500
url: /hi/net/aspose.tasks/projectservermanager/
---
## ProjectServerManager class

वह क्लास जो निर्दिष्ट प्रोजेक्ट ऑनलाइन खाते या निर्दिष्ट ऑन-प्रेमाइस प्रोजेक्ट सर्वर इंस्टेंस (प्रोजेक्ट सर्वर के संस्करण 2016 और 2019 समर्थित हैं) में प्रोजेक्ट्स को पढ़ने और संचालन करने के लिए मेथड्स प्रदान करती है।

```csharp
public sealed class ProjectServerManager
```

## कन्स्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [ProjectServerManager](projectservermanager/)(ProjectServerCredentials) | `ProjectServerManager` क्लास का नया इंस्टेंस इनिशियलाइज़ करता है। |

## विधियाँ

| नाम | विवरण |
| --- | --- |
| [CreateNewProject](../../aspose.tasks/projectservermanager/createnewproject/#createnewproject)(Project) | डिफ़ॉल्ट सहेजने विकल्पों का उपयोग करके Project Server\Project Online इंस्टेंस में नया प्रोजेक्ट बनाता है। |
| [CreateNewProject](../../aspose.tasks/projectservermanager/createnewproject/#createnewproject_1)(Project, ProjectServerSaveOptions) | निर्दिष्ट सहेजने विकल्पों का उपयोग करके Project Server\\Project Online इंस्टेंस में नया प्रोजेक्ट बनाता है। |
| [GetProject](../../aspose.tasks/projectservermanager/getproject/)(Guid) | निर्दिष्ट GUID के साथ प्रोजेक्ट को Project Online खाते \\ Project Server इंस्टेंस से प्राप्त करता है। |
| [GetProjectList](../../aspose.tasks/projectservermanager/getprojectlist/)() | वर्तमान Project Online खाते \\ Project Server इंस्टेंस के 'Working' स्टोर से प्रोजेक्ट्स की सूची प्राप्त करता है। |
| [GetProjectRawData](../../aspose.tasks/projectservermanager/getprojectrawdata/)(Guid) | समस्या निवारण के लिए प्रोजेक्ट का बाइनरी डेटा प्राप्त करता है। |
| [UpdateProject](../../aspose.tasks/projectservermanager/updateproject/#updateproject)(Project) | डिफ़ॉल्ट सहेजने विकल्पों का उपयोग करके Project Server\\Project Online इंस्टेंस में मौजूदा प्रोजेक्ट को अपडेट करता है। मौजूदा प्रोजेक्ट को ओवरराइट किया जाएगा। |
| [UpdateProject](../../aspose.tasks/projectservermanager/updateproject/#updateproject_1)(Project, ProjectServerSaveOptions) | निर्दिष्ट सहेजने विकल्पों का उपयोग करके Project Server\\Project Online इंस्टेंस में मौजूदा प्रोजेक्ट को अपडेट करता है। मौजूदा प्रोजेक्ट को ओवरराइट किया जाएगा। |

## इवेंट्स

| नाम | विवरण |
| --- | --- |
| event [ExecutingWebRequest](../../aspose.tasks/projectservermanager/executingwebrequest/) | एक इवेंट जो तब उठाया जाता है जब वेब अनुरोध Project Server की वेब API को भेजा जाता है। |

## उदाहरण

दिखाता है कि Microsoft Project Online पर पूर्वनिर्धारित सहेजने विकल्पों के साथ नया प्रोजेक्ट बनाने के लिए Project Server मैनेजर का उपयोग कैसे किया जाए।

```csharp
try
{
    const string sharepointDomainAddress = "https://contoso.sharepoint.com/sites/pwa";
    const string UserName = "admin@contoso.onmicrosoft.com";
    const string Password = "MyPassword";

    var credentials = new ProjectServerCredentials(sharepointDomainAddress, UserName, Password);

    var project = new Project(DataDir + @"Project1.mpp");

    var manager = new ProjectServerManager(credentials);
    var options = new ProjectServerSaveOptions
    {
        Timeout = TimeSpan.FromSeconds(10)
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


