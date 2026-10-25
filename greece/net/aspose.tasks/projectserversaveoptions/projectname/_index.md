---
title: "ProjectServerSaveOptions.ProjectName"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα ProjectServerSaveOptions. Λαμβάνει ή ορίζει το όνομα ενός έργου που εμφανίζεται στη λίστα έργων του Project Server / Project Online. Πρέπει να είναι μοναδικό εντός της εγκατάστασης Project Server / Project Online. Εάν παραληφθεί η τιμή, θα χρησιμοποιηθεί η τιμή της ιδιότητας Prj.Name"
type: docs
weight: 40
url: /el/net/aspose.tasks/projectserversaveoptions/projectname/
---
## ProjectServerSaveOptions.ProjectName property

Λαμβάνει ή ορίζει το όνομα ενός έργου που εμφανίζεται στη λίστα έργων του Project Server \ Project Online. Θα πρέπει να είναι μοναδικό εντός του παραδείγματος Project Server \ Project Online. Εάν η τιμή παραλειφθεί, θα χρησιμοποιηθεί η τιμή της ιδιότητας Prj.Name.

```csharp
public string ProjectName { get; set; }
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


