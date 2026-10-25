---
title: "Κλάση ProjectOnlineException"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κλάση Aspose.Tasks.ProjectOnlineException. Αντιπροσωπεύει μια εξαίρεση που ρίχνεται όταν εντοπίζονται σφάλματα κατά την αλληλεπίδραση με το Project Online ή το Project Server."
type: docs
weight: 1480
url: /el/net/aspose.tasks/projectonlineexception/
---
## ProjectOnlineException class

Αντιπροσωπεύει μια εξαίρεση που ρίχνεται όταν εντοπίζονται σφάλματα κατά την αλληλεπίδραση με την υπηρεσία Project Online ή μια παρουσία Project Server.

```csharp
public class ProjectOnlineException : TasksException
```

## Παραδείγματα

Δείχνει πώς να πιάσετε την εξαίρεση κατά την ανάγνωση ενός έργου από το MS Project Online.

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

* class [TasksException](../tasksexception/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


