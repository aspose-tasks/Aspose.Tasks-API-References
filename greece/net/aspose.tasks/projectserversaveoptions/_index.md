---
title: "Κλάση ProjectServerSaveOptions"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κλάση Aspose.Tasks.ProjectServerSaveOptions. Επιτρέπει τον καθορισμό πρόσθετων επιλογών όταν το έργο αποθηκεύεται στο Project Server ή στο Project Online."
type: docs
weight: 1510
url: /el/net/aspose.tasks/projectserversaveoptions/
---
## ProjectServerSaveOptions class

Επιτρέπει τον καθορισμό πρόσθετων επιλογών όταν το έργο αποθηκεύεται στο Project Server ή στο Project Online.

```csharp
public sealed class ProjectServerSaveOptions
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [ProjectServerSaveOptions](projectserversaveoptions/)() | Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης `ProjectServerSaveOptions`. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [PollingInterval](../../aspose.tasks/projectserversaveoptions/pollinginterval/) { get; set; } | Λαμβάνει ή ορίζει το διάστημα μεταξύ των αιτήσεων κατάστασης εργασίας στην ουρά. Η προεπιλεγμένη τιμή είναι 2 δευτερόλεπτα. |
| [ProjectGuid](../../aspose.tasks/projectserversaveoptions/projectguid/) { get; set; } | Λαμβάνει ή ορίζει το μοναδικό αναγνωριστικό ενός έργου. Θα πρέπει να είναι μοναδικό εντός του παραδείγματος Project Server \ Project Online. |
| [ProjectName](../../aspose.tasks/projectserversaveoptions/projectname/) { get; set; } | Λαμβάνει ή ορίζει το όνομα ενός έργου που εμφανίζεται στη λίστα έργων του Project Server \ Project Online. Θα πρέπει να είναι μοναδικό εντός του παραδείγματος Project Server \ Project Online. Εάν η τιμή παραλειφθεί, θα χρησιμοποιηθεί η τιμή της ιδιότητας Prj.Name. |
| [Timeout](../../aspose.tasks/projectserversaveoptions/timeout/) { get; set; } | Λαμβάνει ή ορίζει το χρονικό όριο που χρησιμοποιείται κατά την αναμονή επεξεργασίας του αιτήματος αποθήκευσης έργου από την υπηρεσία επεξεργασίας ουράς του Project Server. Η προεπιλεγμένη τιμή για αυτήν την ιδιότητα είναι 1 λεπτό. |

## Παραδείγματα

Δείχνει πώς να χρησιμοποιήσετε τις επιλογές &lt;see cref=\"Aspose.Tasks.ProjectServerSaveOptions\" /&gt; για να δημιουργήσετε ένα νέο έργο σε τοπικό παράδειγμα του Project Server.

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
    var options = new ProjectServerSaveOptions
                      {
                          ProjectGuid = Guid.NewGuid(),
                          ProjectName = "New project",
                          Timeout = TimeSpan.FromMinutes(5),
                          PollingInterval = TimeSpan.FromSeconds(3)
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


