---
title: "PrimaveraXmlReader.PrimaveraXmlReader"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "PrimaveraXmlReader constructor. Αρχικοποιεί μια νέα παρουσία της κλάσης PrimaveraXmlReader"
type: docs
weight: 10
url: /el/net/aspose.tasks/primaveraxmlreader/primaveraxmlreader/
---
## PrimaveraXmlReader(string) {#constructor_1}

Αρχικοποιεί μια νέα παρουσία της κλάσης [`PrimaveraXmlReader`](../).

```csharp
public PrimaveraXmlReader(string templatePath)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| templatePath | String | Διαδρομή προς το πρότυπο όπου βρίσκεται το έργο Primavera Xml ή τα έργα. |

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

* class [PrimaveraXmlReader](../)
* namespace [Aspose.Tasks](../../primaveraxmlreader/)
* assembly [Aspose.Tasks](../../../)

---

## PrimaveraXmlReader(Stream) {#constructor}

Αρχικοποιεί μια νέα παρουσία της κλάσης [`PrimaveraXmlReader`](../).

```csharp
public PrimaveraXmlReader(Stream stream)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| ροή | Ροή | Ροή που περιέχει περιεχόμενο Primavera Xml. |

## Παραδείγματα

Δείχνει πώς να εισαγάγετε ένα έργο από μια ροή Primavera XML.

```csharp
using (var stream = new FileStream(DataDir + "primavera.xml", FileMode.Open))
{
    var reader = new PrimaveraXmlReader(stream);
    List<int> projectUids = reader.GetProjectUids();
    foreach (var projectUid in projectUids)
    {
        Console.WriteLine("Project UID: " + projectUid);
    }
}
```

### Δείτε επίσης

* class [PrimaveraXmlReader](../)
* namespace [Aspose.Tasks](../../primaveraxmlreader/)
* assembly [Aspose.Tasks](../../../)


