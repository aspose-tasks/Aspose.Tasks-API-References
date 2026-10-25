---
title: "PrimaveraBaseReader.GetProjectUids"
second_title: "Aspose.Tasks für .NET API-Referenz"
description: "PrimaveraBaseReader-Methode. Gibt eine Liste der eindeutigen Kennungen der Projekte zurück."
type: docs
weight: 20
url: /de/net/aspose.tasks/primaverabasereader/getprojectuids/
---
## PrimaveraBaseReader.GetProjectUids method

Gibt eine Liste der eindeutigen Bezeichner der Projekte zurück.

```csharp
public List<int> GetProjectUids()
```

### Rückgabewert

Liste der eindeutigen Kennungen der Projekte.

## Beispiele

Zeigt, wie ein Projekt aus einer Primavera-XML-Datei importiert wird.

```csharp
var reader = new PrimaveraXmlReader(DataDir + "primavera.xml");
List<int> projectUids = reader.GetProjectUids();
foreach (var projectUid in projectUids)
{
    Console.WriteLine("Project UID: " + projectUid);
}
```

### Siehe auch

* class [PrimaveraBaseReader](../)
* namespace [Aspose.Tasks](../../primaverabasereader/)
* assembly [Aspose.Tasks](../../../)


