---
title: "ProjectServerSaveOptions.ProjectGuid"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "ProjectServerSaveOptions प्रॉपर्टी। प्रोजेक्ट का अद्वितीय पहचानकर्ता प्राप्त या सेट करता है। यह Project Server Project Online इंस्टेंस के भीतर अद्वितीय होना चाहिए।"
type: docs
weight: 30
url: /hi/net/aspose.tasks/projectserversaveoptions/projectguid/
---
## ProjectServerSaveOptions.ProjectGuid property

प्रोजेक्ट का अद्वितीय पहचानकर्ता प्राप्त करता है या सेट करता है। यह Project Server \\ Project Online उदाहरण के भीतर अद्वितीय होना चाहिए।

```csharp
public Guid ProjectGuid { get; set; }
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


