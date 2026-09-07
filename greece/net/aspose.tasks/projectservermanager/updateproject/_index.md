---
title: "ProjectServerManager.UpdateProject"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος ProjectServerManager. Ενημερώνει υπάρχον έργο σε παρουσία Project Server/Project Online χρησιμοποιώντας τις προεπιλεγμένες επιλογές αποθήκευσης. Το υπάρχον έργο θα αντικατασταθεί."
type: docs
weight: 70
url: /el/net/aspose.tasks/projectservermanager/updateproject/
---
## UpdateProject(Project) {#updateproject}

Ενημερώνει υπάρχον έργο σε παρουσία Project Server\Project Online χρησιμοποιώντας τις προεπιλεγμένες επιλογές αποθήκευσης. Το υπάρχον έργο θα αντικατασταθεί.

```csharp
public void UpdateProject(Project project)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| project | Project | Το έργο για αποθήκευση σε παρουσία Project Server\Project Online. |

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| [ProjectOnlineException](../../projectonlineexception/) | Σε περίπτωση σφάλματος επικοινωνίας ή σφάλματος που επιστρέφεται από διακομιστή. |

## Παρατηρήσεις

Η ιδιότητα του έργου 'project.Get(Prj.Guid)' πρέπει να είναι ένα έγκυρο guid ενός έργου που υπάρχει στον λογαριασμό Project Server \ Project Online.

## Παραδείγματα

Σε αυτό το παράδειγμα, το έργο φορτώνεται από λογαριασμό Project Online, τροποποιείται και αποθηκεύεται ξανά στον λογαριασμό Project Online.

```csharp
[C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "password");
ProjectServerManager manager = new ProjectServerManager(credentials);
var projectList = manager.GetProjectList();
var projectGuid = projectList.First().Id;
var project = manager.GetProject(projectGuid);
var task = project.RootTask.Children.Add("New task");
manager.UpdateProject(project);
```

Δείχνει πώς να ενημερώσετε το έργο στο Microsoft Project Online.

```csharp
const string URL = "https://contoso.sharepoint.com/sites/pwa";
const string Domain = "CONTOSO.COM";
const string UserName = "Administrator";
const string Password = "MyPassword";

var windowsCredentials = new NetworkCredential(UserName, Password, Domain);
var projectServerCredentials = new ProjectServerCredentials(URL, windowsCredentials);
try
{
    var manager = new ProjectServerManager(projectServerCredentials);

    ProjectInfo projectInfo = null;
    foreach (var info in manager.GetProjectList())
    {
        if (info.Name == "My project")
        {
            projectInfo = info;
        }
    }

    if (projectInfo == null)
    {
        Console.WriteLine("Project 'My project' not found in working store of Project Online account.");
        return;
    }

    var project = manager.GetProject(projectInfo.Id);
    project.Set(Prj.FinishDate, new DateTime(2020, 03, 01));

    var task = project.RootTask.Children.Add("New task");
    task.Set(Tsk.Start, new DateTime(2020, 02, 26));
    task.Set(Tsk.Duration, project.GetDuration(2, TimeUnitType.Day));

    manager.UpdateProject(project);
}
catch (ProjectOnlineException ex)
{
    Console.WriteLine("Failed to update the project. Error: " + ex);
}
```

### Δείτε επίσης

* class [Project](../../project/)
* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)

---

## UpdateProject(Project, ProjectServerSaveOptions) {#updateproject_1}

Ενημερώνει υπάρχον έργο σε παρουσία Project Server\Project Online χρησιμοποιώντας τις καθορισμένες επιλογές αποθήκευσης. Το υπάρχον έργο θα αντικατασταθεί.

```csharp
public void UpdateProject(Project project, ProjectServerSaveOptions saveOptions)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| project | Project | Το έργο για αποθήκευση σε παρουσία Project Server\Project Online. |
| saveOptions | ProjectServerSaveOptions | Παράδειγμα της κλάσης [`ProjectServerSaveOptions`](../../projectserversaveoptions/). |

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| [ProjectOnlineException](../../projectonlineexception/) | Σε περίπτωση σφάλματος επικοινωνίας ή σφάλματος που επιστρέφεται από διακομιστή. |

## Παρατηρήσεις

Το saveOptions.ProjectGuid πρέπει να οριστεί σε ένα guid ενός έργου που υπάρχει στην παρουσία Project Server\ Project Online.

## Παραδείγματα

Σε αυτό το παράδειγμα, το έργο φορτώνεται από λογαριασμό Project Online, τροποποιείται και αποθηκεύεται ξανά στον λογαριασμό Project Online.

```csharp
[C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "password");
ProjectServerManager manager = new ProjectServerManager(credentials);
var projectList = manager.GetProjectList();
var projectGuid = projectList.First().Id;
var project = manager.GetProject(projectGuid);
var task = project.RootTask.Children.Add("New task");
manager.UpdateProject(project, new ProjectServerSaveOptions
{
    ProjectGuid = projectGuid
});
```

Δείχνει πώς να ενημερώσετε το έργο στο Microsoft Project Online χρησιμοποιώντας τις επιλογές αποθήκευσης του Project Server.

```csharp
const string SharepointDomainAddress = "https://contoso.sharepoint.com/sites/pwa";
const string UserName = "admin@contoso.onmicrosoft.com";
const string Password = "MyPassword";

var credentials = new ProjectServerCredentials(SharepointDomainAddress, UserName, Password);

try
{
    var manager = new ProjectServerManager(credentials);

    ProjectInfo projectInfo = null;
    foreach (var info in manager.GetProjectList())
    {
        if (info.Name == "My project")
        {
            projectInfo = info;
        }
    }

    if (projectInfo == null)
    {
        Console.WriteLine("Project 'My project' not found in working store of Project Online account.");
        return;
    }

    var project = manager.GetProject(projectInfo.Id);
    project.Set(Prj.FinishDate, new DateTime(2020, 03, 01));

    var task = project.RootTask.Children.Add("New task");
    task.Set(Tsk.Start, new DateTime(2020, 02, 26));
    task.Set(Tsk.Duration, project.GetDuration(2, TimeUnitType.Day));

    var options = new ProjectServerSaveOptions { Timeout = TimeSpan.FromMinutes(5) };

    manager.UpdateProject(project, options);
}
catch (ProjectOnlineException ex)
{
    Console.WriteLine("Failed to update the project. Error: " + ex);
}
```

### Δείτε επίσης

* class [Project](../../project/)
* class [ProjectServerSaveOptions](../../projectserversaveoptions/)
* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)


