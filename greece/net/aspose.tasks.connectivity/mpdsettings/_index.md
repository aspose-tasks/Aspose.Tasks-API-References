---
title: "Κλάση MpdSettings"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.Connectivity.MpdSettings class. Επιτρέπει τον καθορισμό των απαραίτητων επιλογών για την ανάγνωση δεδομένων έργου από τη μορφή αρχείου MPD της βάσης δεδομένων MS Access"
type: docs
weight: 300
url: /el/net/aspose.tasks.connectivity/mpdsettings/
---
## MpdSettings class

Επιτρέπει τον καθορισμό των απαραίτητων επιλογών για ανάγνωση δεδομένων έργου από τη μορφή MPD (μορφή αρχείου βάσης δεδομένων MS Access).

```csharp
public class MpdSettings : DbSettings
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [MpdSettings](mpdsettings/)(string, int) | Αρχικοποιεί μια νέα παρουσία της κλάσης `MpdSettings`. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [ConnectionString](../../aspose.tasks.connectivity/dbsettings/connectionstring/) { get; set; } | Λαμβάνει ή ορίζει τη συμβολοσειρά σύνδεσης. |
| [ProjectId](../../aspose.tasks.connectivity/mpdsettings/projectid/) { get; } | Λαμβάνει το id του έργου για ανάγνωση. |
| [ProjectLoadingCallback](../../aspose.tasks.connectivity/dbsettings/projectloadingcallback/) { get; set; } | Λαμβάνει ή ορίζει την κλήση επιστροφής που θα κληθεί κατά τη διάρκεια των λειτουργιών φόρτωσης έργου. |
| [ProviderFactory](../../aspose.tasks.connectivity/dbsettings/providerfactory/) { get; set; } | Λαμβάνει ή ορίζει μια παρουσία του DbProviderFactory που χρησιμοποιείται για σύνδεση με τη βάση δεδομένων. Εάν οριστούν και τα ProviderFactory και ProviderInvariantName, το ProviderFactory έχει προτεραιότητα. Η προεπιλεγμένη τιμή είναι null. |
| [ProviderInvariantName](../../aspose.tasks.connectivity/dbsettings/providerinvariantname/) { get; set; } | Λαμβάνει ή ορίζει το αμετάβλητο όνομα του παρόχου που χρησιμοποιείται για τη λήψη μιας παρουσίασης της κλάσης DbProviderFactory. Η προεπιλεγμένη τιμή είναι SqlClient. |

## Παραδείγματα

Δείχνει πώς να χρησιμοποιήσετε τις ρυθμίσεις MPD για να ελέγξετε την εισαγωγή του έργου από τη βάση δεδομένων.

```csharp
var settings = new MpdSettings("Provider=Microsoft.Jet.OLEDB.4.0; Data Source=" + DataDir + "MpdFileToRead.mpd", 1);

Console.WriteLine("Project ID to load: " + settings.ProjectId);

var project = new Project(settings);
Console.WriteLine(project.Get(Prj.Name));
```

### Δείτε επίσης

* class [DbSettings](../dbsettings/)
* namespace [Aspose.Tasks.Connectivity](../../aspose.tasks.connectivity/)
* assembly [Aspose.Tasks](../../)


