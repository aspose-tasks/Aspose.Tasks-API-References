---
title: "Κλάση MspDbSettings"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.Connectivity.MspDbSettings class. Επιτρέπει τον καθορισμό των απαραίτητων επιλογών για την ανάγνωση δεδομένων έργου από τη βάση δεδομένων του MS Project Server"
type: docs
weight: 310
url: /el/net/aspose.tasks.connectivity/mspdbsettings/
---
## MspDbSettings class

Επιτρέπει τον καθορισμό των απαραίτητων επιλογών για ανάγνωση δεδομένων έργου από τη βάση δεδομένων του MS Project Server.

```csharp
public class MspDbSettings : DbSettings
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [MspDbSettings](mspdbsettings/)(string, Guid) | Αρχικοποιεί μια νέα παρουσία της κλάσης `MspDbSettings`. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [ConnectionString](../../aspose.tasks.connectivity/dbsettings/connectionstring/) { get; set; } | Λαμβάνει ή ορίζει τη συμβολοσειρά σύνδεσης. |
| [ProjectGuid](../../aspose.tasks.connectivity/mspdbsettings/projectguid/) { get; } | Λαμβάνει το guid του έργου για ανάγνωση. |
| [ProjectLoadingCallback](../../aspose.tasks.connectivity/dbsettings/projectloadingcallback/) { get; set; } | Λαμβάνει ή ορίζει την κλήση επιστροφής που θα κληθεί κατά τη διάρκεια των λειτουργιών φόρτωσης έργου. |
| [ProviderFactory](../../aspose.tasks.connectivity/dbsettings/providerfactory/) { get; set; } | Λαμβάνει ή ορίζει μια παρουσία του DbProviderFactory που χρησιμοποιείται για σύνδεση με τη βάση δεδομένων. Εάν οριστούν και τα ProviderFactory και ProviderInvariantName, το ProviderFactory έχει προτεραιότητα. Η προεπιλεγμένη τιμή είναι null. |
| [ProviderInvariantName](../../aspose.tasks.connectivity/dbsettings/providerinvariantname/) { get; set; } | Λαμβάνει ή ορίζει το αμετάβλητο όνομα του παρόχου που χρησιμοποιείται για τη λήψη μιας παρουσίασης της κλάσης DbProviderFactory. Η προεπιλεγμένη τιμή είναι SqlClient. |
| [Schema](../../aspose.tasks.connectivity/mspdbsettings/schema/) { get; set; } | Λαμβάνει ή ορίζει το σχήμα του MS Project Server. Η προεπιλεγμένη τιμή είναι "pub". |

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

* class [DbSettings](../dbsettings/)
* namespace [Aspose.Tasks.Connectivity](../../aspose.tasks.connectivity/)
* assembly [Aspose.Tasks](../../)


