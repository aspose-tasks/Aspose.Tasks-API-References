---
title: "ProjectServerCredentials.SiteUrl"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية ProjectServerCredentials. يحصل على عنوان URL الخاص بـ PWA في موقع SharePoint أو عنوان URL لخادم Project Server المحلي. على سبيل المثال https//your_company_name.sharepoint.com/sites/pwa"
type: docs
weight: 30
url: /ar/net/aspose.tasks/projectservercredentials/siteurl/
---
## ProjectServerCredentials.SiteUrl property

يحصل على عنوان URL لـ PWA في موقع SharePoint أو عنوان URL لـ Project Server المحلي. على سبيل المثال، https://your_company_name.sharepoint.com/sites/pwa";

```csharp
public string SiteUrl { get; }
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


