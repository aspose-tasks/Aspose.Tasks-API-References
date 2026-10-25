---
title: "ProjectServerSaveOptions.PollingInterval"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα ProjectServerSaveOptions. Λαμβάνει ή ορίζει το διάστημα μεταξύ αιτήσεων κατάστασης εργασίας στην ουρά. Η προεπιλεγμένη τιμή είναι 2 δευτερόλεπτα"
type: docs
weight: 20
url: /el/net/aspose.tasks/projectserversaveoptions/pollinginterval/
---
## ProjectServerSaveOptions.PollingInterval property

Λαμβάνει ή ορίζει το διάστημα μεταξύ των αιτήσεων κατάστασης εργασίας στην ουρά. Η προεπιλεγμένη τιμή είναι 2 δευτερόλεπτα.

```csharp
public TimeSpan PollingInterval { get; set; }
```

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

* class [ProjectServerSaveOptions](../)
* namespace [Aspose.Tasks](../../projectserversaveoptions/)
* assembly [Aspose.Tasks](../../../)


