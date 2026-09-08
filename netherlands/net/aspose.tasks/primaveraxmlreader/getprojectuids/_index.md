---
title: "GetProjectUids"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Retourneer een lijst met de unieke identifiers van de projecten."
type: docs
weight: 20
url: /nl/net/aspose.tasks/primaveraxmlreader/getprojectuids/
---
## PrimaveraXmlReader.GetProjectUids method

Retourneer een lijst met de unieke identificatoren van de projecten.

```csharp
public List<int> GetProjectUids()
```

### Retourwaarde

Lijst met unieke identifiers van projecten.

### Voorbeelden

Toont hoe een project te importeren vanuit een Primavera XML‑bestand.

```csharp
var reader = new PrimaveraXmlReader(DataDir + "primavera.xml");
List<int> projectUids = reader.GetProjectUids();
foreach (var projectUid in projectUids)
{
    Console.WriteLine("Project UID: " + projectUid);
}
```

### Zie ook

* class [PrimaveraXmlReader](../../primaveraxmlreader)
* namespace [Aspose.Tasks](../../primaveraxmlreader)
* assembly [Aspose.Tasks](../../../)

<!-- NIET BEWERKEN: gegenereerd door xmldocmd voor Aspose.Tasks.dll -->
