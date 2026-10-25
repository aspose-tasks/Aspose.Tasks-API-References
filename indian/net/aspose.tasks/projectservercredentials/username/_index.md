---
title: "ProjectServerCredentials.UserName"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "ProjectServerCredentials प्रॉपर्टी। SharePoint साइट के लिए उपयोगकर्ता नाम प्राप्त करता है।"
type: docs
weight: 40
url: /hi/net/aspose.tasks/projectservercredentials/username/
---
## ProjectServerCredentials.UserName property

SharePoint साइट के लिए उपयोगकर्ता नाम प्राप्त करता है।

```csharp
public string UserName { get; }
```

## उदाहरण

दिखाता है कि कैसे Project Server क्रेडेंशियल्स को SharePointOnlineCredentials के साथ उपयोग करके Microsoft Project Online में प्रोजेक्ट बनाया जाए।

```csharp
try
{
    const string Username = "admin@contoso.onmicrosoft.com";
    const string SecuredPassword = "MyPassword";
    var url = new Uri("https://contoso.sharepoint.com/sites/pwa");
    var project = new Project(DataDir + "Project1.mpp");
    var password = new SecureString();
    foreach (var c in SecuredPassword)
    {
        password.AppendChar(c);
    }

    var onlineCredentials = new SharePointOnlineCredentials(Username, password);
    var projectServerCredentials = new ProjectServerCredentials(url.ToString(), onlineCredentials.GetAuthenticationCookie(url, true));

    Console.WriteLine("Project Server Auth Token: " + projectServerCredentials.AuthToken);
    Console.WriteLine("Project Server Site Url: " + projectServerCredentials.SiteUrl);
    Console.WriteLine("Project Server User Name: " + projectServerCredentials.UserName);

    var manager = new ProjectServerManager(projectServerCredentials);
    manager.CreateNewProject(project);
}
catch (ProjectOnlineException ex)
{
    Console.WriteLine(ex.Message);
}
```

### संबंधित देखें

* class [ProjectServerCredentials](../)
* namespace [Aspose.Tasks](../../projectservercredentials/)
* assembly [Aspose.Tasks](../../../)


