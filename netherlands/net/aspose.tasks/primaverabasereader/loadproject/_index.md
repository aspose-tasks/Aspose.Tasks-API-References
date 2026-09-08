---
title: "PrimaveraBaseReader.LoadProject"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "PrimaveraBaseReader methode. Laadt het project met de opgegeven unieke identifier"
type: docs
weight: 30
url: /nl/net/aspose.tasks/primaverabasereader/loadproject/
---
## PrimaveraBaseReader.LoadProject method

Laadt het project met de opgegeven unieke identificator.

```csharp
public virtual Project LoadProject(int projectUid)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| projectUid | Int32 | Unieke identifier van het te laden project. |

### Retourwaarde

Project met opgegeven unieke identifier uit het opgegeven multi‑projectbestand. Null als het project niet bestaat.

## Voorbeelden

Toont hoe een project te laden vanuit een Primavera XML‑bestand wanneer de project‑uid bekend is.

```csharp
var reader = new PrimaveraXmlReader(DataDir + "PrimaveraProject.xml");
var project = reader.LoadProject(3882);
Console.WriteLine(project.Name);
```

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

* class [Project](../../project/)
* class [PrimaveraBaseReader](../)
* namespace [Aspose.Tasks](../../primaverabasereader/)
* assembly [Aspose.Tasks](../../../)


