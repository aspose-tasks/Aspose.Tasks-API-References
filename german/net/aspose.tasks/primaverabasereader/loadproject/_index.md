---
title: "PrimaveraBaseReader.LoadProject"
second_title: "Aspose.Tasks für .NET API-Referenz"
description: "PrimaveraBaseReader-Methode. Lädt das Projekt mit der angegebenen eindeutigen Kennung"
type: docs
weight: 30
url: /de/net/aspose.tasks/primaverabasereader/loadproject/
---
## PrimaveraBaseReader.LoadProject method

Lädt das Projekt mit dem angegebenen eindeutigen Bezeichner.

```csharp
public virtual Project LoadProject(int projectUid)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| projectUid | Int32 | Eindeutige Kennung des zu ladenden Projekts. |

### Rückgabewert

Projekt mit der angegebenen eindeutigen Kennung aus der angegebenen Mehrprojektdatei. Null, wenn das Projekt nicht existiert.

## Beispiele

Zeigt, wie man ein Projekt aus einer Primavera XML-Datei lädt, wenn die Projekt‑UID bekannt ist.

```csharp
var reader = new PrimaveraXmlReader(DataDir + "PrimaveraProject.xml");
var project = reader.LoadProject(3882);
Console.WriteLine(project.Name);
```

Zeigt, wie man Kurzprojekte-Informationen aus einer Primavera XER-Datei untersucht.

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

### Siehe auch

* class [Project](../../project/)
* class [PrimaveraBaseReader](../)
* namespace [Aspose.Tasks](../../primaverabasereader/)
* assembly [Aspose.Tasks](../../../)


