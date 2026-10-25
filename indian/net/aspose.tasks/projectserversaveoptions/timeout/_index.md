---
title: "ProjectServerSaveOptions.Timeout"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "ProjectServerSaveOptions प्रॉपर्टी। प्रोजेक्ट सर्वर की कतार प्रोसेसिंग सेवा द्वारा सहेजने के अनुरोध की प्रोसेसिंग की प्रतीक्षा करते समय उपयोग होने वाला टाइमआउट प्राप्त या सेट करता है। इस प्रॉपर्टी का डिफ़ॉल्ट मान 1 मिनट है।"
type: docs
weight: 50
url: /hi/net/aspose.tasks/projectserversaveoptions/timeout/
---
## ProjectServerSaveOptions.Timeout property

Project Server की क्यू प्रोसेसिंग सेवा द्वारा प्रोजेक्ट सहेजने के अनुरोध की प्रोसेसिंग की प्रतीक्षा करते समय उपयोग किए जाने वाले टाइमआउट को प्राप्त करता है या सेट करता है। इस प्रॉपर्टी का डिफ़ॉल्ट मान 1 मिनट है।

```csharp
public TimeSpan Timeout { get; set; }
```

## टिप्पणियाँ

बड़े प्रोजेक्ट्स के लिए या जब Project Server इंस्टेंस अन्य अनुरोधों का जवाब देने में बहुत व्यस्त हो, तो प्रोसेसिंग समय अधिक हो सकता है।

## उदाहरण

Microsoft Project Online पर प्रोजेक्ट को अपडेट करने और सहेजने के टाइमआउट मान को नियंत्रित करने का तरीका दिखाता है।

```csharp
const string SharepointDomainAddress = "https://contoso.sharepoint.com/sites/pwa";
const string UserName = "admin@contoso.onmicrosoft.com";
const string Password = "MyPassword";

var credentials = new ProjectServerCredentials(SharepointDomainAddress, UserName, Password);
try
{
    var manager = new ProjectServerManager(credentials);

    ProjectInfo projectInfo = null;
    foreach (var info in manager.GetProjectList())
    {
        if (info.Name == "My project")
        {
            projectInfo = info;
        }
    }

    if (projectInfo == null)
    {
        Console.WriteLine("Project 'My project' not found in working store of Project Online account.");
        return;
    }

    var project = manager.GetProject(projectInfo.Id);
    project.Set(Prj.FinishDate, new DateTime(2020, 03, 01));

    var task = project.RootTask.Children.Add("New task");
    task.Set(Tsk.Start, new DateTime(2020, 02, 26));
    task.Set(Tsk.Duration, project.GetDuration(2, TimeUnitType.Day));

    var options = new ProjectServerSaveOptions { Timeout = TimeSpan.FromMinutes(5) };

    manager.UpdateProject(project, options);
}
catch (ProjectOnlineException ex)
{
    Console.WriteLine("Failed to update the project. Error: " + ex);
}
```

### संबंधित देखें

* class [ProjectServerSaveOptions](../)
* namespace [Aspose.Tasks](../../projectserversaveoptions/)
* assembly [Aspose.Tasks](../../../)


