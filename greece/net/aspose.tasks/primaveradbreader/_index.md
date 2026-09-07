---
title: "Κλάση PrimaveraDbReader"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κλάση Aspose.Tasks.PrimaveraDbReader. Αντιπροσωπεύει έναν αναγνώστη για την ανάγνωση πληροφοριών έργου από τη βάση δεδομένων Primavera."
type: docs
weight: 1350
url: /el/net/aspose.tasks/primaveradbreader/
---
## PrimaveraDbReader class

Αντιπροσωπεύει έναν αναγνώστη για την ανάγνωση πληροφοριών έργου από τη βάση δεδομένων Primavera

```csharp
public sealed class PrimaveraDbReader : PrimaveraBaseReader
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [PrimaveraDbReader](primaveradbreader/)(PrimaveraDbSettings) | Αρχικοποιεί μια νέα παρουσία της κλάσης [`PrimaveraXerReader`](../primaveraxerreader/). |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| [GetProjectInfos](../../aspose.tasks/primaverabasereader/getprojectinfos/)() | Επιστρέφει μια λίστα με τα σύντομα αντικείμενα πληροφοριών του έργου. |
| [GetProjectUids](../../aspose.tasks/primaverabasereader/getprojectuids/)() | Επιστρέψτε μια λίστα με τα μοναδικά αναγνωριστικά των έργων. |
| override [LoadProject](../../aspose.tasks/primaveradbreader/loadproject/)(int) | Φορτώνει το έργο με το καθορισμένο μοναδικό αναγνωριστικό. |

## Παραδείγματα

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

* class [PrimaveraBaseReader](../primaverabasereader/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


