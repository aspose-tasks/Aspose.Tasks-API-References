---
title: "ProjectServerSaveOptions.Timeout"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα ProjectServerSaveOptions. Λαμβάνει ή ορίζει το χρονικό όριο που χρησιμοποιείται κατά την αναμονή επεξεργασίας του αιτήματος αποθήκευσης έργου από την υπηρεσία επεξεργασίας ουράς του Project Server. Η προεπιλεγμένη τιμή για αυτή την ιδιότητα είναι 1 λεπτό"
type: docs
weight: 50
url: /el/net/aspose.tasks/projectserversaveoptions/timeout/
---
## ProjectServerSaveOptions.Timeout property

Λαμβάνει ή ορίζει το χρονικό όριο που χρησιμοποιείται κατά την αναμονή επεξεργασίας του αιτήματος αποθήκευσης έργου από την υπηρεσία επεξεργασίας ουράς του Project Server. Η προεπιλεγμένη τιμή για αυτήν την ιδιότητα είναι 1 λεπτό.

```csharp
public TimeSpan Timeout { get; set; }
```

## Παρατηρήσεις

Ο χρόνος επεξεργασίας μπορεί να είναι μεγαλύτερος για μεγάλα έργα ή σε περίπτωση που η εγκατάσταση του Project Server είναι πολύ απασχολημένη να ανταποκριθεί σε άλλα αιτήματα.

## Παραδείγματα

Δείχνει πώς να ενημερώσετε ένα έργο στο Microsoft Project Online και να ελέγξετε την τιμή του χρονικού ορίου αποθήκευσης.

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

* class [ProjectServerSaveOptions](../)
* namespace [Aspose.Tasks](../../projectserversaveoptions/)
* assembly [Aspose.Tasks](../../../)


