---
title: "Κλάση PrimaveraDbSettings"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.Connectivity.PrimaveraDbSettings class. Επιτρέπει τον καθορισμό των απαραίτητων επιλογών για την ανάγνωση δεδομένων έργου από τη βάση δεδομένων Primavera"
type: docs
weight: 320
url: /el/net/aspose.tasks.connectivity/primaveradbsettings/
---
## PrimaveraDbSettings class

Επιτρέπει τον καθορισμό των απαραίτητων επιλογών για ανάγνωση δεδομένων έργου από τη βάση δεδομένων Primavera.

```csharp
public class PrimaveraDbSettings : DbSettings
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [PrimaveraDbSettings](primaveradbsettings/)(string, int) | Αρχικοποιεί μια νέα παρουσία της κλάσης `PrimaveraDbSettings`. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [ConnectionString](../../aspose.tasks.connectivity/dbsettings/connectionstring/) { get; set; } | Λαμβάνει ή ορίζει τη συμβολοσειρά σύνδεσης. |
| [ProjectId](../../aspose.tasks.connectivity/primaveradbsettings/projectid/) { get; } | Λαμβάνει το id του έργου για ανάγνωση. |
| [ProjectLoadingCallback](../../aspose.tasks.connectivity/dbsettings/projectloadingcallback/) { get; set; } | Λαμβάνει ή ορίζει την κλήση επιστροφής που θα κληθεί κατά τη διάρκεια των λειτουργιών φόρτωσης έργου. |
| [ProviderFactory](../../aspose.tasks.connectivity/dbsettings/providerfactory/) { get; set; } | Λαμβάνει ή ορίζει μια παρουσία του DbProviderFactory που χρησιμοποιείται για σύνδεση με τη βάση δεδομένων. Εάν οριστούν και τα ProviderFactory και ProviderInvariantName, το ProviderFactory έχει προτεραιότητα. Η προεπιλεγμένη τιμή είναι null. |
| [ProviderInvariantName](../../aspose.tasks.connectivity/dbsettings/providerinvariantname/) { get; set; } | Λαμβάνει ή ορίζει το αμετάβλητο όνομα του παρόχου που χρησιμοποιείται για τη λήψη μιας παρουσίασης της κλάσης DbProviderFactory. Η προεπιλεγμένη τιμή είναι SqlClient. |

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

Δείχνει πώς να λάβετε σύντομες πληροφορίες των έργων από μια βάση δεδομένων Primavera.

```csharp
var settings = new PrimaveraDbSettings(GetConnectionString(), 0);

var reader = new PrimaveraDbReader(settings);
var projectInfos = reader.GetProjectInfos();

foreach (var info in projectInfos)
{
    Console.WriteLine("{0} - '{1}' - '{2}'", info.Uid, info.ShortName, info.Name);
}

var firstProject = reader.LoadProject(projectInfos[0].Uid);
Console.WriteLine(firstProject.Uid);
Console.WriteLine(firstProject.Name);
Console.WriteLine(firstProject.PrimaveraProperties.ShortName);
```

### Δείτε επίσης

* class [DbSettings](../dbsettings/)
* namespace [Aspose.Tasks.Connectivity](../../aspose.tasks.connectivity/)
* assembly [Aspose.Tasks](../../)


