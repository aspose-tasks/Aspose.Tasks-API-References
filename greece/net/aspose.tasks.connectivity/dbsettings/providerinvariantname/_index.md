---
title: "DbSettings.ProviderInvariantName"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "DbSettings property. Λαμβάνει ή ορίζει το όνομα αμετάβλητου παρόχου που χρησιμοποιείται για τη λήψη μιας παρουσίας της κλάσης DbProviderFactory. Η προεπιλεγμένη τιμή είναι SqlClient."
type: docs
weight: 40
url: /el/net/aspose.tasks.connectivity/dbsettings/providerinvariantname/
---
## DbSettings.ProviderInvariantName property

Λαμβάνει ή ορίζει το αμετάβλητο όνομα του παρόχου που χρησιμοποιείται για τη λήψη μιας παρουσίασης της κλάσης DbProviderFactory. Η προεπιλεγμένη τιμή είναι SqlClient.

```csharp
public string ProviderInvariantName { get; set; }
```

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

* class [DbSettings](../)
* namespace [Aspose.Tasks.Connectivity](../../dbsettings/)
* assembly [Aspose.Tasks](../../../)


