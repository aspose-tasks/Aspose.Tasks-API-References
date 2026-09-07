---
title: "ProjectServerSaveOptions.PollingInterval"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "ProjectServerSaveOptions प्रॉपर्टी। कतार जॉब स्थिति अनुरोधों के बीच अंतराल प्राप्त या सेट करता है। डिफ़ॉल्ट मान 2 सेकंड है।"
type: docs
weight: 20
url: /hi/net/aspose.tasks/projectserversaveoptions/pollinginterval/
---
## ProjectServerSaveOptions.PollingInterval property

क्यू जॉब स्थिति अनुरोधों के बीच अंतराल प्राप्त करता है या सेट करता है। डिफ़ॉल्ट मान 2 सेकंड है।

```csharp
public TimeSpan PollingInterval { get; set; }
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


