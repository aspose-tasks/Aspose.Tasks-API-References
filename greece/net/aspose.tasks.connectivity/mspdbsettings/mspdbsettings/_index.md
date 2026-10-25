---
title: "MspDbSettings.MspDbSettings"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κατασκευαστής MspDbSettings. Αρχικοποιεί ένα νέο αντικείμενο της κλάσης MspDbSettings."
type: docs
weight: 10
url: /el/net/aspose.tasks.connectivity/mspdbsettings/mspdbsettings/
---
## MspDbSettings constructor

Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [`MspDbSettings`](../).

```csharp
public MspDbSettings(string connectionString, Guid projectGuid)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| connectionString | String | η καθορισμένη συμβολοσειρά σύνδεσης. |
| projectGuid | Guid | το καθορισμένο guid ενός έργου για ανάγνωση. |

## Παραδείγματα

Δείχνει πώς να εισάγετε ένα έργο από μια βάση δεδομένων.

```csharp
try
{
    // Δημιουργία συμβολοσειράς σύνδεσης
    var connectionString = new SqlConnectionStringBuilder();
    connectionString.DataSource = "192.168.56.2,1433";
    connectionString.Encrypt = true;
    connectionString.TrustServerCertificate = true;
    connectionString.InitialCatalog = "ProjectServer_Published";
    connectionString.NetworkLibrary = "DBMSSOCN";
    connectionString.UserID = "sa";
    connectionString.Password = "*****";

    // δημιουργία ρυθμίσεων για φόρτωση από τη βάση δεδομένων MS
    var settings = new MspDbSettings(connectionString.ConnectionString, new Guid("E6426C44-D6CB-4B9C-AF16-48910ACE0F54"));
    settings.Schema = "dbo";

    Console.WriteLine("Project GUID to load: " + settings.ProjectGuid);

    var project = new Project(settings);

    project.Save(OutDir + "ImportProjectDataFromDatabase_out.mpp", SaveFileFormat.Mpp);
}
catch (Exception ex)
{
    Console.WriteLine(ex.Message + " Please setup proper data source (DataSource, InitialCatalog etc)");
}
```

### Δείτε επίσης

* class [MspDbSettings](../)
* namespace [Aspose.Tasks.Connectivity](../../mspdbsettings/)
* assembly [Aspose.Tasks](../../../)


