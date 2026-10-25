---
title: "ProjectServerSaveOptions.ProjectServerSaveOptions"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κατασκευαστής ProjectServerSaveOptions. Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης ProjectServerSaveOptions"
type: docs
weight: 10
url: /el/net/aspose.tasks/projectserversaveoptions/projectserversaveoptions/
---
## ProjectServerSaveOptions constructor

Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης [`ProjectServerSaveOptions`](../).

```csharp
public ProjectServerSaveOptions()
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


