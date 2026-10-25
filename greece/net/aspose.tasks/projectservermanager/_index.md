---
title: "Κλάση ProjectServerManager"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κλάση Aspose.Tasks.ProjectServerManager. Η κλάση που παρέχει τις μεθόδους για ανάγνωση και εκτέλεση λειτουργιών σε έργα στον καθορισμένο λογαριασμό Project Online ή στην καθορισμένη εγκατάσταση on-premise Project Server. Υποστηρίζονται εκδόσεις Project Server 2016 και 2019."
type: docs
weight: 1500
url: /el/net/aspose.tasks/projectservermanager/
---
## ProjectServerManager class

Η κλάση που παρέχει τις μεθόδους για ανάγνωση και εκτέλεση λειτουργιών σε έργα στον καθορισμένο λογαριασμό Project Online ή στην καθορισμένη τοπική παρουσία του Project Server (υποστηρίζονται οι εκδόσεις 2016 και 2019 του Project Server).

```csharp
public sealed class ProjectServerManager
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [ProjectServerManager](projectservermanager/)(ProjectServerCredentials) | Αρχικοποιεί μια νέα παρουσία της κλάσης `ProjectServerManager`. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| [CreateNewProject](../../aspose.tasks/projectservermanager/createnewproject/#createnewproject)(Project) | Δημιουργεί νέο έργο σε εγκατάσταση Project Server\\Project Online χρησιμοποιώντας τις προεπιλεγμένες επιλογές αποθήκευσης. |
| [CreateNewProject](../../aspose.tasks/projectservermanager/createnewproject/#createnewproject_1)(Project, ProjectServerSaveOptions) | Δημιουργεί νέο έργο σε παρουσία Project Server\Project Online χρησιμοποιώντας τις καθορισμένες επιλογές αποθήκευσης. |
| [GetProject](../../aspose.tasks/projectservermanager/getproject/)(Guid) | Αποκτά το έργο με το καθορισμένο guid από τον λογαριασμό Project Online \ Project Server παρουσία. |
| [GetProjectList](../../aspose.tasks/projectservermanager/getprojectlist/)() | Αποκτά τη λίστα των έργων από το αποθετήριο 'Working' του τρέχοντος λογαριασμού Project Online \ Project Server παρουσία. |
| [GetProjectRawData](../../aspose.tasks/projectservermanager/getprojectrawdata/)(Guid) | Αποκτά τα δυαδικά δεδομένα του έργου για σκοπούς αντιμετώπισης προβλημάτων. |
| [UpdateProject](../../aspose.tasks/projectservermanager/updateproject/#updateproject)(Project) | Ενημερώνει υπάρχον έργο σε παρουσία Project Server\Project Online χρησιμοποιώντας τις προεπιλεγμένες επιλογές αποθήκευσης. Το υπάρχον έργο θα αντικατασταθεί. |
| [UpdateProject](../../aspose.tasks/projectservermanager/updateproject/#updateproject_1)(Project, ProjectServerSaveOptions) | Ενημερώνει υπάρχον έργο σε παρουσία Project Server\Project Online χρησιμοποιώντας τις καθορισμένες επιλογές αποθήκευσης. Το υπάρχον έργο θα αντικατασταθεί. |

## Συμβάντα

| Όνομα | Περιγραφή |
| --- | --- |
| event [ExecutingWebRequest](../../aspose.tasks/projectservermanager/executingwebrequest/) | Ένα συμβάν που ενεργοποιείται όταν το web request αποστέλλεται στο web API του Project Server. |

## Παραδείγματα

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


