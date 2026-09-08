---
title: "PrimaveraXerReader.PrimaveraXerReader"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "PrimaveraXerReader constructor. Initialiseert een nieuw exemplaar van de PrimaveraXerReader-klasse"
type: docs
weight: 10
url: /nl/net/aspose.tasks/primaveraxerreader/primaveraxerreader/
---
## PrimaveraXerReader(string) {#constructor_1}

Initialiseert een nieuw exemplaar van de [`PrimaveraXerReader`](../) klasse.

```csharp
public PrimaveraXerReader(string xerFilePath)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| xerFilePath | String | Pad naar .xer‑bestand waar het Primavera‑project of de projecten zich bevinden. |

## Voorbeelden

Toont hoe de informatie van korte projecten uit een Primavera XER‑bestand kan worden onderzocht.

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

### Zie ook

* class [PrimaveraXerReader](../)
* namespace [Aspose.Tasks](../../primaveraxerreader/)
* assembly [Aspose.Tasks](../../../)

---

## PrimaveraXerReader(Stream) {#constructor}

Initialiseert een nieuw exemplaar van de [`PrimaveraXerReader`](../) klasse.

```csharp
public PrimaveraXerReader(Stream stream)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| stroom | Stroom | Stream met Primavera XER-inhoud. |

### Zie ook

* class [PrimaveraXerReader](../)
* namespace [Aspose.Tasks](../../primaveraxerreader/)
* assembly [Aspose.Tasks](../../../)


