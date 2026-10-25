---
title: "ProjectServerSaveOptions.ProjectName"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "ProjectServerSaveOptions प्रॉपर्टी। Project Server Project Online प्रोजेक्ट सूची में प्रदर्शित होने वाले प्रोजेक्ट का नाम प्राप्त या सेट करता है। यह Project Server Project Online इंस्टेंस के भीतर अद्वितीय होना चाहिए। यदि यह मान छोड़ा जाता है तो Prj.Name प्रॉपर्टी का मान उपयोग किया जाएगा।"
type: docs
weight: 40
url: /hi/net/aspose.tasks/projectserversaveoptions/projectname/
---
## ProjectServerSaveOptions.ProjectName property

Project Server \\ Project Online प्रोजेक्ट सूची में प्रदर्शित होने वाले प्रोजेक्ट का नाम प्राप्त करता है या सेट करता है। यह Project Server \\ Project Online उदाहरण के भीतर अद्वितीय होना चाहिए। यदि मान छोड़ा जाता है, तो Prj.Name प्रॉपर्टी का मान उपयोग किया जाएगा।

```csharp
public string ProjectName { get; set; }
```

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

* class [ProjectServerSaveOptions](../)
* namespace [Aspose.Tasks](../../projectserversaveoptions/)
* assembly [Aspose.Tasks](../../../)


