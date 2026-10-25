---
title: "ProjectServerSaveOptions.ProjectGuid"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα ProjectServerSaveOptions. Λαμβάνει ή ορίζει το μοναδικό αναγνωριστικό ενός έργου. Πρέπει να είναι μοναδικό εντός της εγκατάστασης Project Server / Project Online"
type: docs
weight: 30
url: /el/net/aspose.tasks/projectserversaveoptions/projectguid/
---
## ProjectServerSaveOptions.ProjectGuid property

Λαμβάνει ή ορίζει το μοναδικό αναγνωριστικό ενός έργου. Θα πρέπει να είναι μοναδικό εντός του παραδείγματος Project Server \ Project Online.

```csharp
public Guid ProjectGuid { get; set; }
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


