---
title: "PrimaveraDbSettings.PrimaveraDbSettings"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κατασκευαστής PrimaveraDbSettings. Αρχικοποιεί μια νέα παρουσία της κλάσης PrimaveraDbSettings."
type: docs
weight: 10
url: /el/net/aspose.tasks.connectivity/primaveradbsettings/primaveradbsettings/
---
## PrimaveraDbSettings constructor

Αρχικοποιεί μια νέα παρουσία της κλάσης [`PrimaveraDbSettings`](../).

```csharp
public PrimaveraDbSettings(string connectionString, int projectId)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| connectionString | String | η καθορισμένη συμβολοσειρά σύνδεσης. |
| projectId | Int32 | το καθορισμένο id ενός έργου για ανάγνωση. |

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


