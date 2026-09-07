---
title: "ProjectServerCredentials.ProjectServerCredentials"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "ProjectServerCredentials κατασκευαστής. Αρχικοποιεί μια νέα παρουσία της κλάσης ProjectServerCredentials χρησιμοποιώντας το URL του ιστότοπου SharePoint και έγκυρο διακριτικό εξουσιοδότησης SPOIDCRL για τον ιστότοπο PWA Project Web Access του SharePoint"
type: docs
weight: 10
url: /el/net/aspose.tasks/projectservercredentials/projectservercredentials/
---
## ProjectServerCredentials(string, string) {#constructor_1}

Αρχικοποιεί μια νέα παρουσία της κλάσης [`ProjectServerCredentials`](../) χρησιμοποιώντας το URL του ιστότοπου SharePoint και έγκυρο διακριτικό εξουσιοδότησης SPOIDCRL για τον ιστότοπο PWA (Project Web Access) του SharePoint.

```csharp
public ProjectServerCredentials(string siteUrl, string authToken)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| siteUrl | String | Το URL του API PWA (Project Web Access) του Project Online. |
| authToken | String | Το διακριτικό εξουσιοδότησης (SPOIDCRL) για τον ιστότοπο PWA (Project Web Access) του SharePoint. |

## Παρατηρήσεις

Χρησιμοποιήστε αυτόν τον κατασκευαστή για να συνδεθείτε στο ProjectOnline όταν έχετε ήδη AuthToken για τον ιστότοπο SharePoint Online σας.

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

---

## ProjectServerCredentials(string, string, string) {#constructor_2}

Αρχικοποιεί μια νέα παρουσία της κλάσης [`ProjectServerCredentials`](../) χρησιμοποιώντας τη διεύθυνση URL του ιστότοπου SharePoint, το όνομα χρήστη και τον κωδικό πρόσβασης.

```csharp
public ProjectServerCredentials(string siteUrl, string userName, string password)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| siteUrl | String | Το URL του API PWA (Project Web Access) του Project Online. |
| userName | String | Το όνομα χρήστη για τον ιστότοπο SharePoint. |
| password | String | Ο κωδικός πρόσβασης για τον ιστότοπο SharePoint. |

## Παρατηρήσεις

Χρησιμοποιήστε αυτόν τον κατασκευαστή για να συνδεθείτε στο ProjectOnline. Παρακαλώ σημειώστε ότι η κληρονομική πιστοποίηση πρέπει να είναι ενεργοποιημένη στην Azure portal και στο κέντρο διαχείρισης Office 365.

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

* class [ProjectServerCredentials](../)
* namespace [Aspose.Tasks](../../projectservercredentials/)
* assembly [Aspose.Tasks](../../../)

---

## ProjectServerCredentials(string, NetworkCredential) {#constructor}

Αρχικοποιεί μια νέα παρουσία της κλάσης [`ProjectServerCredentials`](../) χρησιμοποιώντας τη διεύθυνση URL του τελικού σημείου Project Web Access και τα διαπιστευτήρια δικτύου.

```csharp
public ProjectServerCredentials(string siteUrl, NetworkCredential credentials)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| siteUrl | String | Η διεύθυνση URL του τελικού σημείου project web access. |
| διαπιστευτήρια | NetworkCredential | Τα διαπιστευτήρια που χρησιμοποιούνται για σύνδεση στο τελικό σημείο Project Web Access. |

## Παρατηρήσεις

Χρησιμοποιήστε αυτόν τον κατασκευαστή για να συνδεθείτε σε τοπική (on-premise) παρουσία του Project Server μέσω PWA.

## Παραδείγματα

Σε αυτό το παράδειγμα η παρουσία της κλάσης [`ProjectServerManager`](../../projectservermanager/) χρησιμοποιείται για την ανάγνωση λίστας έργων από την παρουσία του Project Server που βρίσκεται στο http://project_server_instance.local

```csharp
string site = "http://project_server_instance.local/sites/pwa";
var windowsCredentials = new NetworkCredential("Administrator", "my_password", "DOMAIN");
var projectServerCredentials = new ProjectServerCredentials(site, windowsCredentials);
ProjectServerManager manager = new ProjectServerManager(projectServerCredentials);

var list = manager.GetProjectList();
foreach (var projectInfo in list)
{
    Console.WriteLine("{0} - {1} - {2}", projectInfo.Id, projectInfo.CreatedDate, projectInfo.Name);
}
```

Δείχνει πώς να χρησιμοποιήσετε τα διαπιστευτήρια του Project Server μαζί με τα διαπιστευτήρια δικτύου για να διαβάσετε ένα έργο από τοπική (on-premise) παρουσία του Project Server.

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


