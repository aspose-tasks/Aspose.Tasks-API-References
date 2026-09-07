---
title: "Κλάση PrimaveraXmlReader"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.PrimaveraXmlReader κλάση. Αντιπροσωπεύει έναν αναγνώστη που επιτρέπει την ανάκτηση των UID του έργου από αρχείο Primavera Xml"
type: docs
weight: 1400
url: /el/net/aspose.tasks/primaveraxmlreader/
---
## PrimaveraXmlReader class

Αντιπροσωπεύει έναν αναγνώστη που επιτρέπει την ανάκτηση UID έργων από αρχείο Primavera Xml.

```csharp
public class PrimaveraXmlReader : PrimaveraBaseReader
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [PrimaveraXmlReader](primaveraxmlreader/#constructor)(Stream) | Αρχικοποιεί μια νέα παρουσία της `PrimaveraXmlReader` κλάσης. |
| [PrimaveraXmlReader](primaveraxmlreader/#constructor_1)(string) | Αρχικοποιεί μια νέα παρουσία της `PrimaveraXmlReader` κλάσης. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| [GetProjectInfos](../../aspose.tasks/primaverabasereader/getprojectinfos/)() | Επιστρέφει μια λίστα με τα σύντομα αντικείμενα πληροφοριών του έργου. |
| [GetProjectUids](../../aspose.tasks/primaverabasereader/getprojectuids/)() | Επιστρέψτε μια λίστα με τα μοναδικά αναγνωριστικά των έργων. |
| virtual [LoadProject](../../aspose.tasks/primaverabasereader/loadproject/)(int) | Φορτώνει το έργο με το καθορισμένο μοναδικό αναγνωριστικό. |

## Παραδείγματα

Δείχνει πώς να εξετάσετε τις πληροφορίες σύντομων έργων από ένα αρχείο Primavera XML.

```csharp
var reader = new PrimaveraXmlReader(DataDir + "MultiprojectWithExternal.xml");
var projectInfos = reader.GetProjectInfos();
foreach (var info in projectInfos)
{
    Console.WriteLine("{0} - '{1}' - {2}", info.Uid, info.Name, info.ExportFlag);
}
```

### Δείτε επίσης

* class [PrimaveraBaseReader](../primaverabasereader/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


