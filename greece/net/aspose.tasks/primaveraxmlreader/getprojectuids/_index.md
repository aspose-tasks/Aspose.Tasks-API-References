---
title: "GetProjectUids"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Επιστρέφει μια λίστα με τα μοναδικά αναγνωριστικά των έργων."
type: docs
weight: 20
url: /el/net/aspose.tasks/primaveraxmlreader/getprojectuids/
---
## PrimaveraXmlReader.GetProjectUids method

Επιστρέψτε μια λίστα με τα μοναδικά αναγνωριστικά των έργων.

```csharp
public List<int> GetProjectUids()
```

### Τιμή Επιστροφής

Λίστα με τα μοναδικά αναγνωριστικά των έργων.

### Παραδείγματα

Δείχνει πώς να εισάγετε ένα έργο από ένα αρχείο Primavera XML.

```csharp
var reader = new PrimaveraXmlReader(DataDir + "primavera.xml");
List<int> projectUids = reader.GetProjectUids();
foreach (var projectUid in projectUids)
{
    Console.WriteLine("Project UID: " + projectUid);
}
```

### Δείτε επίσης

* class [PrimaveraXmlReader](../../primaveraxmlreader)
* namespace [Aspose.Tasks](../../primaveraxmlreader)
* assembly [Aspose.Tasks](../../../)

<!-- ΜΗ ΕΠΕΞΕΡΓΑΣΙΑ: δημιουργήθηκε από xmldocmd για Aspose.Tasks.dll -->
