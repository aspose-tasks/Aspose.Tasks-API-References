---
title: "GetProjectUids"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Restituisce un elenco degli identificatori univoci dei progetti."
type: docs
weight: 20
url: /it/net/aspose.tasks/primaveraxmlreader/getprojectuids/
---
## PrimaveraXmlReader.GetProjectUids method

Restituisci un elenco degli identificatori univoci dei progetti.

```csharp
public List<int> GetProjectUids()
```

### Valore di ritorno

Elenco degli identificatori univoci dei progetti.

### Esempi

Mostra come importare un progetto da un file XML Primavera.

```csharp
var reader = new PrimaveraXmlReader(DataDir + "primavera.xml");
List<int> projectUids = reader.GetProjectUids();
foreach (var projectUid in projectUids)
{
    Console.WriteLine("Project UID: " + projectUid);
}
```

### Vedi anche

* class [PrimaveraXmlReader](../../primaveraxmlreader)
* namespace [Aspose.Tasks](../../primaveraxmlreader)
* assembly [Aspose.Tasks](../../../)

<!-- NON MODIFICARE: generato da xmldocmd per Aspose.Tasks.dll -->
