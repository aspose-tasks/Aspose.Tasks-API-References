---
title: "ProjectServerManager.ExecutingWebRequest"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "ProjectServerManager इवेंट। एक इवेंट जो तब उठाया जाता है जब वेब अनुरोध Project Servers वेब API को भेजा जाता है।"
type: docs
weight: 20
url: /hi/net/aspose.tasks/projectservermanager/executingwebrequest/
---
## ProjectServerManager.ExecutingWebRequest event

एक इवेंट जो तब उठाया जाता है जब वेब अनुरोध Project Server की वेब API को भेजा जाता है।

```csharp
public event EventHandler<WebRequestEventArgs> ExecutingWebRequest;
```

## उदाहरण

ProjectServerManager.ExecutingWebRequest इवेंट का उपयोग करके Project Server को भेजे गए वेब अनुरोधों को कस्टमाइज़ करने का तरीका दर्शाता है।

```csharp
try
{
    const string SiteUrl = "https://myprojectserver/sites/pwa";
    const string UserName = "test_user";
    const string Password = "MyPassword";

    var credentials = new ProjectServerCredentials(SiteUrl, new NetworkCredential(UserName, Password));

    var project = new Project(DataDir + @"Project1.mpp");

    var manager = new ProjectServerManager(credentials);
    manager.ExecutingWebRequest += delegate (object sender, WebRequestEventArgs e)
    {
        e.WebRequest.Headers.Add("XMyCustomHeader", "testvalue");
    };

    var list = manager.GetProjectList();
}
catch (ProjectOnlineException ex)
{
    Console.WriteLine(ex.Message);
}
```

### संबंधित देखें

* class [WebRequestEventArgs](../../webrequesteventargs/)
* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)


