---
title: "DbSettings.ProviderFactory"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα DbSettings. Λαμβάνει ή ορίζει μια παρουσία του DbProviderFactory που χρησιμοποιείται για σύνδεση στη βάση δεδομένων. Εάν τόσο το ProviderFactory όσο και το ProviderInvariantName έχουν οριστεί, το ProviderFactory έχει προτεραιότητα. Η προεπιλεγμένη τιμή είναι null."
type: docs
weight: 30
url: /el/net/aspose.tasks.connectivity/dbsettings/providerfactory/
---
## DbSettings.ProviderFactory property

Λαμβάνει ή ορίζει μια παρουσία του DbProviderFactory που χρησιμοποιείται για σύνδεση με τη βάση δεδομένων. Εάν οριστούν και τα ProviderFactory και ProviderInvariantName, το ProviderFactory έχει προτεραιότητα. Η προεπιλεγμένη τιμή είναι null.

```csharp
public DbProviderFactory ProviderFactory { get; set; }
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

* class [DbSettings](../)
* namespace [Aspose.Tasks.Connectivity](../../dbsettings/)
* assembly [Aspose.Tasks](../../../)


