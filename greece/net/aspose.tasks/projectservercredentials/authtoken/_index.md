---
title: "ProjectServerCredentials.AuthToken"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "ProjectServerCredentials ιδιότητα. Λαμβάνει το διακριτικό εξουσιοδότησης για το παράδειγμα SharePoint"
type: docs
weight: 20
url: /el/net/aspose.tasks/projectservercredentials/authtoken/
---
## ProjectServerCredentials.AuthToken property

Λαμβάνει το διακριτικό εξουσιοδότησης για την παρουσία του SharePoint.

```csharp
public string AuthToken { get; }
```

## Παραδείγματα

Δείχνει πώς να χρησιμοποιήσετε τα διαπιστευτήρια Project Server με SharePointOnlineCredentials για να δημιουργήσετε έργο στο Microsoft Project Online.

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

### Δείτε επίσης

* class [ProjectServerCredentials](../)
* namespace [Aspose.Tasks](../../projectservercredentials/)
* assembly [Aspose.Tasks](../../../)


