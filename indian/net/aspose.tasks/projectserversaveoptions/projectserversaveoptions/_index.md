---
title: "ProjectServerSaveOptions.ProjectServerSaveOptions"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "ProjectServerSaveOptions कंस्ट्रक्टर। ProjectServerSaveOptions क्लास का नया इंस्टेंस प्रारंभ करता है।"
type: docs
weight: 10
url: /hi/net/aspose.tasks/projectserversaveoptions/projectserversaveoptions/
---
## ProjectServerSaveOptions constructor

[`ProjectServerSaveOptions`](../) क्लास का नया इंस्टेंस प्रारंभ करता है।

```csharp
public ProjectServerSaveOptions()
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


