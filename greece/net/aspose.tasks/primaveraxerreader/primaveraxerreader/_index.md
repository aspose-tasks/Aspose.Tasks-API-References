---
title: "PrimaveraXerReader.PrimaveraXerReader"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κατασκευαστής PrimaveraXerReader. Αρχικοποιεί ένα νέο αντικείμενο της κλάσης PrimaveraXerReader"
type: docs
weight: 10
url: /el/net/aspose.tasks/primaveraxerreader/primaveraxerreader/
---
## PrimaveraXerReader(string) {#constructor_1}

Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [`PrimaveraXerReader`](../).

```csharp
public PrimaveraXerReader(string xerFilePath)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| xerFilePath | String | Διαδρομή προς το αρχείο .xer όπου βρίσκεται το έργο ή τα έργα Primavera. |

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

* class [PrimaveraXerReader](../)
* namespace [Aspose.Tasks](../../primaveraxerreader/)
* assembly [Aspose.Tasks](../../../)

---

## PrimaveraXerReader(Stream) {#constructor}

Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [`PrimaveraXerReader`](../).

```csharp
public PrimaveraXerReader(Stream stream)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| ροή | Ροή | Ροή με περιεχόμενο Primavera XER. |

### Δείτε επίσης

* class [PrimaveraXerReader](../)
* namespace [Aspose.Tasks](../../primaveraxerreader/)
* assembly [Aspose.Tasks](../../../)


