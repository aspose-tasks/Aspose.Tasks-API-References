---
title: "PrimaveraXmlReader.PrimaveraXmlReader"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "PrimaveraXmlReader‑constructor. Initialiseert een nieuw exemplaar van de PrimaveraXmlReader‑klasse."
type: docs
weight: 10
url: /nl/net/aspose.tasks/primaveraxmlreader/primaveraxmlreader/
---
## PrimaveraXmlReader(string) {#constructor_1}

Initialiseert een nieuw exemplaar van de [`PrimaveraXmlReader`](../) klasse.

```csharp
public PrimaveraXmlReader(string templatePath)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| templatePath | String | Pad naar de sjabloon waar het Primavera Xml-project of -projecten zich bevinden |

## Voorbeelden

Toont hoe korte projectinformatie te onderzoeken uit een Primavera XML‑bestand.

```csharp
var reader = new PrimaveraXmlReader(DataDir + "MultiprojectWithExternal.xml");
var projectInfos = reader.GetProjectInfos();
foreach (var info in projectInfos)
{
    Console.WriteLine("{0} - '{1}' - {2}", info.Uid, info.Name, info.ExportFlag);
}
```

### Zie ook

* class [PrimaveraXmlReader](../)
* namespace [Aspose.Tasks](../../primaveraxmlreader/)
* assembly [Aspose.Tasks](../../../)

---

## PrimaveraXmlReader(Stream) {#constructor}

Initialiseert een nieuw exemplaar van de [`PrimaveraXmlReader`](../) klasse.

```csharp
public PrimaveraXmlReader(Stream stream)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| stroom | Stroom | Stream met Primavera Xml-inhoud. |

## Voorbeelden

Toont hoe een project te importeren vanuit een Primavera XML-stream.

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

### Zie ook

* class [PrimaveraXmlReader](../)
* namespace [Aspose.Tasks](../../primaveraxmlreader/)
* assembly [Aspose.Tasks](../../../)


