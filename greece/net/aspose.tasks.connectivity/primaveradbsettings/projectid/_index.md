---
title: "PrimaveraDbSettings.ProjectId"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα PrimaveraDbSettings. Λαμβάνει το αναγνωριστικό του έργου που θα διαβαστεί."
type: docs
weight: 20
url: /el/net/aspose.tasks.connectivity/primaveradbsettings/projectid/
---
## PrimaveraDbSettings.ProjectId property

Λαμβάνει το id του έργου για ανάγνωση.

```csharp
public int ProjectId { get; }
```

## Παραδείγματα

Δείχνει πώς να εισάγετε ένα έργο από μια βάση δεδομένων Primavera.

```csharp
// Αρχικοποιήστε μια νέα παρουσία της κλάσης PrimaveraDbSettings με τη συμβολοσειρά σύνδεσης και το id του έργου
var settings = new PrimaveraDbSettings(GetConnectionString(), 4502);
settings.ProviderFactory = SqliteFactory.Instance;

Console.WriteLine("Project UID to read: " + settings.ProjectId);

// διαβάστε το έργο με UID = 4502
var project = new Project(settings);
Console.WriteLine(project.Uid);
Console.WriteLine(project.Name);
Console.WriteLine(project.PrimaveraProperties.ShortName);
```

### Δείτε επίσης

* class [PrimaveraDbSettings](../)
* namespace [Aspose.Tasks.Connectivity](../../primaveradbsettings/)
* assembly [Aspose.Tasks](../../../)


