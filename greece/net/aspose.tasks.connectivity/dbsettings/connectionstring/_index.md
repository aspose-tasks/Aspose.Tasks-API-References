---
title: "DbSettings.ConnectionString"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "DbSettings property. Λαμβάνει ή ορίζει τη συμβολοσειρά σύνδεσης."
type: docs
weight: 10
url: /el/net/aspose.tasks.connectivity/dbsettings/connectionstring/
---
## DbSettings.ConnectionString property

Λαμβάνει ή ορίζει τη συμβολοσειρά σύνδεσης.

```csharp
public string ConnectionString { get; set; }
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


