---
title: "PrimaveraBaseReader.GetProjectUids"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "PrimaveraBaseReader methode. Retourneert een lijst met de unieke identifiers van de projecten"
type: docs
weight: 20
url: /nl/net/aspose.tasks/primaverabasereader/getprojectuids/
---
## PrimaveraBaseReader.GetProjectUids method

Retourneer een lijst met de unieke identificatoren van de projecten.

```csharp
public List<int> GetProjectUids()
```

### Retourwaarde

Lijst met unieke identifiers van projecten.

## Voorbeelden

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

* class [PrimaveraBaseReader](../)
* namespace [Aspose.Tasks](../../primaverabasereader/)
* assembly [Aspose.Tasks](../../../)


