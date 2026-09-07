---
title: "ProjectServerManager.CreateNewProject"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος ProjectServerManager. Δημιουργεί νέο έργο σε παρουσία του Project ServerProject Online χρησιμοποιώντας τις προεπιλεγμένες επιλογές αποθήκευσης."
type: docs
weight: 30
url: /el/net/aspose.tasks/projectservermanager/createnewproject/
---
## CreateNewProject(Project) {#createnewproject}

Δημιουργεί νέο έργο σε εγκατάσταση Project Server\\Project Online χρησιμοποιώντας τις προεπιλεγμένες επιλογές αποθήκευσης.

```csharp
public void CreateNewProject(Project project)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| project | Project | Το έργο για αποθήκευση σε παρουσία Project Server\Project Online. |

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| [ProjectOnlineException](../../projectonlineexception/) | Σε περίπτωση σφάλματος επικοινωνίας ή σφάλματος που επιστρέφεται από διακομιστή. |

## Παραδείγματα

Σε αυτό το παράδειγμα το έργο φορτώνεται από αρχείο .mpp και αποθηκεύεται σε λογαριασμό Project Online.

```csharp
[C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "password");
var project = new Project(@"sample.mpp");
ProjectServerManager manager = new ProjectServerManager(credentials);
manager.CreateNewProject(project);
```

Δείχνει πώς να χρησιμοποιήσετε το ProjectServerManager για να δημιουργήσετε ένα νέο έργο στο Microsoft Project Online.

```csharp
try
{
    const string SharepointDomainAddress = "https://contoso.sharepoint.com/sites/pwa";
    const string UserName = "admin@contoso.onmicrosoft.com";
    const string Password = "MyPassword";

    var credentials = new ProjectServerCredentials(SharepointDomainAddress, UserName, Password);

    var project = new Project(DataDir + @"Project1.mpp");

    var manager = new ProjectServerManager(credentials);
    manager.CreateNewProject(project);
}
catch (ProjectOnlineException ex)
{
    Console.WriteLine(ex.Message);
}
```

### Δείτε επίσης

* class [Project](../../project/)
* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)

---

## CreateNewProject(Project, ProjectServerSaveOptions) {#createnewproject_1}

Δημιουργεί νέο έργο σε παρουσία Project Server\Project Online χρησιμοποιώντας τις καθορισμένες επιλογές αποθήκευσης.

```csharp
public void CreateNewProject(Project project, ProjectServerSaveOptions saveOptions)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| project | Project | Το έργο για αποθήκευση σε παρουσία Project Server\Project Online. |
| saveOptions | ProjectServerSaveOptions | Παράδειγμα της κλάσης [`ProjectServerSaveOptions`](../../projectserversaveoptions/). |

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| [ProjectOnlineException](../../projectonlineexception/) | Σε περίπτωση σφάλματος επικοινωνίας ή σφάλματος που επιστρέφεται από διακομιστή. |

## Παραδείγματα

Σε αυτό το παράδειγμα το έργο φορτώνεται από αρχείο .mpp και αποθηκεύεται σε λογαριασμό Project Online.

```csharp
[C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "password");
var project = new Project(@"sample.mpp");
ProjectServerManager manager = new ProjectServerManager(credentials);
manager.CreateNewProject(project, new ProjectServerSaveOptions
{
    ProjectName = "My new project"
});
```

Δείχνει πώς να χρησιμοποιήσετε το Project Server manager για να δημιουργήσετε ένα νέο έργο με προορισμένες επιλογές αποθήκευσης στο Microsoft Project Online.

```csharp
try
{
    const string sharepointDomainAddress = "https://contoso.sharepoint.com/sites/pwa";
    const string UserName = "admin@contoso.onmicrosoft.com";
    const string Password = "MyPassword";

    var credentials = new ProjectServerCredentials(sharepointDomainAddress, UserName, Password);

    var project = new Project(DataDir + @"Project1.mpp");

    var manager = new ProjectServerManager(credentials);
    var options = new ProjectServerSaveOptions
    {
        Timeout = TimeSpan.FromSeconds(10)
    };
    manager.CreateNewProject(project, options);
}
catch (ProjectOnlineException ex)
{
    Console.WriteLine(ex.Message);
}
```

### Δείτε επίσης

* class [Project](../../project/)
* class [ProjectServerSaveOptions](../../projectserversaveoptions/)
* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)


