---
title: "ProjectServerCredentials.AuthToken"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية ProjectServerCredentials. يحصل على رمز التفويض لمثيل SharePoint"
type: docs
weight: 20
url: /ar/net/aspose.tasks/projectservercredentials/authtoken/
---
## ProjectServerCredentials.AuthToken property

يحصل على رمز التفويض لنسخة SharePoint.

```csharp
public string AuthToken { get; }
```

## الأمثلة

يوضح كيفية استخدام بيانات اعتماد Project Server مع SharePointOnlineCredentials لإنشاء مشروع في Microsoft Project Online.

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

### انظر أيضًا

* class [ProjectServerCredentials](../)
* namespace [Aspose.Tasks](../../projectservercredentials/)
* assembly [Aspose.Tasks](../../../)


