---
title: "Κλάση ProjectServerCredentials"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κλάση Aspose.Tasks.ProjectServerCredentials. Διαπιστευτήρια που χρησιμοποιούνται για σύνδεση με το Project Online ή το τοπικό (on‑premise) αντίγραφο του Project Server."
type: docs
weight: 1490
url: /el/net/aspose.tasks/projectservercredentials/
---
## ProjectServerCredentials class

Διαπιστευτήρια που χρησιμοποιούνται για τη σύνδεση με το Project Online ή την τοπική παρουσία του Project Server.

```csharp
public sealed class ProjectServerCredentials
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [ProjectServerCredentials](projectservercredentials/#constructor)(string, NetworkCredential) | Αρχικοποιεί μια νέα παρουσία της κλάσης `ProjectServerCredentials` χρησιμοποιώντας το URL του τελικού σημείου Project Web Access και τα διαπιστευτήρια δικτύου. |
| [ProjectServerCredentials](projectservercredentials/#constructor_1)(string, string) | Αρχικοποιεί μια νέα παρουσία της κλάσης `ProjectServerCredentials` χρησιμοποιώντας το URL του ιστότοπου SharePoint και ένα έγκυρο διακριτικό εξουσιοδότησης SPOIDCRL για τον ιστότοπο PWA (Project Web Access) του SharePoint. |
| [ProjectServerCredentials](projectservercredentials/#constructor_2)(string, string, string) | Αρχικοποιεί μια νέα παρουσία της κλάσης `ProjectServerCredentials` χρησιμοποιώντας το URL του ιστότοπου SharePoint, το όνομα χρήστη και τον κωδικό πρόσβασης. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [AuthToken](../../aspose.tasks/projectservercredentials/authtoken/) { get; } | Λαμβάνει το διακριτικό εξουσιοδότησης για την παρουσία του SharePoint. |
| [SiteUrl](../../aspose.tasks/projectservercredentials/siteurl/) { get; } | Λαμβάνει το URL του PWA στον ιστότοπο SharePoint ή το URL του τοπικού Project Server. Για παράδειγμα, https://your_company_name.sharepoint.com/sites/pwa\"; |
| [UserName](../../aspose.tasks/projectservercredentials/username/) { get; } | Λαμβάνει το όνομα χρήστη για τον ιστότοπο SharePoint. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| override [ToString](../../aspose.tasks/projectservercredentials/tostring/)() | Επιστρέφει μια αναπαράσταση string αυτής της παρουσίας. |

## Παραδείγματα

Δείχνει πώς να χρησιμοποιήσετε τα διαπιστευτήρια του project server για την ανάκτηση λίστας έργων από το Microsoft Project Online.

```csharp
try
{
    const string SharepointDomainAddress = "https://contoso.sharepoint.com/sites/pwa";
    const string UserName = "admin@contoso.onmicrosoft.com";
    const string Password = "MyPassword";

    var credentials = new ProjectServerCredentials(SharepointDomainAddress, UserName, Password);

    var newProject = new Project(DataDir + @"Project1.mpp");

    var manager = new ProjectServerManager(credentials);
    manager.CreateNewProject(newProject);

    IEnumerable<ProjectInfo> list = manager.GetProjectList();

    foreach (var info in list)
    {
        var project = manager.GetProject(info.Id);
        Console.WriteLine("{0} - {1} - {2}", info.Name, info.CreatedDate, info.LastSavedDate);
        Console.WriteLine("Resources count: {0}", project.Resources.Count);
    }
}
catch (ProjectOnlineException ex)
{
    Console.WriteLine(ex.Message);
}
```

### Δείτε επίσης

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


