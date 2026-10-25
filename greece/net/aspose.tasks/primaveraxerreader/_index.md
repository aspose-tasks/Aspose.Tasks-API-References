---
title: "Κλάση PrimaveraXerReader"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κλάση Aspose.Tasks.PrimaveraXerReader. Αντιπροσωπεύει έναν αναγνώστη για την ανάγνωση των UID του έργου από το αρχείο Primavera XER."
type: docs
weight: 1390
url: /el/net/aspose.tasks/primaveraxerreader/
---
## PrimaveraXerReader class

Αντιπροσωπεύει έναν αναγνώστη για την ανάγνωση UID έργων από αρχείο Primavera XER

```csharp
public sealed class PrimaveraXerReader : PrimaveraBaseReader
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [PrimaveraXerReader](primaveraxerreader/#constructor)(Stream) | Αρχικοποιεί μια νέα παρουσία της κλάσης `PrimaveraXerReader`. |
| [PrimaveraXerReader](primaveraxerreader/#constructor_1)(string) | Αρχικοποιεί μια νέα παρουσία της κλάσης `PrimaveraXerReader`. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| [GetProjectInfos](../../aspose.tasks/primaverabasereader/getprojectinfos/)() | Επιστρέφει μια λίστα με τα σύντομα αντικείμενα πληροφοριών του έργου. |
| [GetProjectUids](../../aspose.tasks/primaverabasereader/getprojectuids/)() | Επιστρέψτε μια λίστα με τα μοναδικά αναγνωριστικά των έργων. |
| virtual [LoadProject](../../aspose.tasks/primaverabasereader/loadproject/)(int) | Φορτώνει το έργο με το καθορισμένο μοναδικό αναγνωριστικό. |

## Παραδείγματα

Δείχνει πώς να εξετάσετε τις πληροφορίες σύντομων έργων από ένα αρχείο Primavera XER.

```csharp
var reader = new PrimaveraXerReader(DataDir + "MultiprojectWithExternal.xer");
var projectInfos = reader.GetProjectInfos();
foreach (var info in projectInfos)
{
    Console.WriteLine("{0} - '{1}' - {2}", info.Uid, info.Name, info.ExportFlag);
}

var project = reader.LoadProject(5494);

Console.WriteLine("Loaded project '{0}' with Uid {1}", project.Name, project.Uid);
```

### Δείτε επίσης

* class [PrimaveraBaseReader](../primaverabasereader/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


