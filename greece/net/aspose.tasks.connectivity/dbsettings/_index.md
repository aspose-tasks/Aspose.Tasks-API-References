---
title: "Κλάση DbSettings"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.Connectivity.DbSettings class. Επιτρέπει τον καθορισμό ρυθμίσεων για την ανάγνωση από τη βάση δεδομένων του έργου"
type: docs
weight: 290
url: /el/net/aspose.tasks.connectivity/dbsettings/
---
## DbSettings class

Επιτρέπει τον καθορισμό ρυθμίσεων για ανάγνωση από τη βάση δεδομένων του έργου.

```csharp
public abstract class DbSettings
```

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [ConnectionString](../../aspose.tasks.connectivity/dbsettings/connectionstring/) { get; set; } | Λαμβάνει ή ορίζει τη συμβολοσειρά σύνδεσης. |
| [ProjectLoadingCallback](../../aspose.tasks.connectivity/dbsettings/projectloadingcallback/) { get; set; } | Λαμβάνει ή ορίζει την κλήση επιστροφής που θα κληθεί κατά τη διάρκεια των λειτουργιών φόρτωσης έργου. |
| [ProviderFactory](../../aspose.tasks.connectivity/dbsettings/providerfactory/) { get; set; } | Λαμβάνει ή ορίζει μια παρουσία του DbProviderFactory που χρησιμοποιείται για σύνδεση με τη βάση δεδομένων. Εάν οριστούν και τα ProviderFactory και ProviderInvariantName, το ProviderFactory έχει προτεραιότητα. Η προεπιλεγμένη τιμή είναι null. |
| [ProviderInvariantName](../../aspose.tasks.connectivity/dbsettings/providerinvariantname/) { get; set; } | Λαμβάνει ή ορίζει το αμετάβλητο όνομα του παρόχου που χρησιμοποιείται για τη λήψη μιας παρουσίασης της κλάσης DbProviderFactory. Η προεπιλεγμένη τιμή είναι SqlClient. |

## Παραδείγματα

Δείχνει πώς να διαβάσετε ένα έργο από ένα αρχείο Primavera XML με πολλαπλά έργα χρησιμοποιώντας το όνομα του παρόχου.

```csharp
var connectionString = "Data Source=" + DataDir + "\\PPMDBSQLite.db";

// Δημιουργία ρυθμίσεων Primavera DB χρησιμοποιώντας τη συμβολοσειρά σύνδεσης και το id του έργου
var settings = new PrimaveraDbSettings(connectionString, 4502);
settings.ProviderInvariantName = "System.Data.SQLite";

Console.WriteLine("Connection String: " + settings.ConnectionString);
Console.WriteLine("Provider Name: " + settings.ProviderInvariantName);

var project = new Project(settings);
project.Save(OutDir + "SupportForSQLiteDatabase_out.mpp", SaveFileFormat.Mpp);
```

### Δείτε επίσης

* namespace [Aspose.Tasks.Connectivity](../../aspose.tasks.connectivity/)
* assembly [Aspose.Tasks](../../)


