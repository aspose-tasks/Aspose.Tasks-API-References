---
title: "Project.GetProjectFileInfo"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Project-methode. Lees projectbestandsinformatie uit het bestand"
type: docs
weight: 1280
url: /nl/net/aspose.tasks/project/getprojectfileinfo/
---
## GetProjectFileInfo(string) {#getprojectfileinfo_1}

Leest projectbestandsinformatie uit het bestand.

```csharp
public static ProjectFileInfo GetProjectFileInfo(string filename)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| bestandsnaam | String | De projectbestandsnaam. |

### Retourwaarde

De projectbestandsinformatie [`ProjectFileInfo`](../../projectfileinfo/).

## Voorbeelden

Toont hoe projectbestandsinformatie werd gelezen uit een XML-bestand.

```csharp
var info = Project.GetProjectFileInfo(DataDir + "Project.xml");
Console.WriteLine("CanRead: " + info.CanRead);
Console.WriteLine("ProjectApplicationInfo: " + info.ProjectApplicationInfo);
Console.WriteLine("ProjectFileFormat: " + info.ProjectFileFormat);
```

### Zie ook

* class [ProjectFileInfo](../../projectfileinfo/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetProjectFileInfo(Stream) {#getprojectfileinfo}

Haalt projectbestandsinformatie op uit de stream.

```csharp
public static ProjectFileInfo GetProjectFileInfo(Stream stream)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| stroom | Stroom | De gegevensstroom. |

### Retourwaarde

De projectbestandsinformatie [`ProjectFileInfo`](../../projectfileinfo/).

## Voorbeelden

Toont hoe u projectbestandsinformatie van een XML‑bestand die uit een stream is gelezen, kunt lezen.

```csharp
using (var stream = new FileStream(DataDir + "Project.xml", FileMode.Open))
{
    var info = Project.GetProjectFileInfo(stream);
    Console.WriteLine("CanRead: " + info.CanRead);
    Console.WriteLine("ProjectApplicationInfo: " + info.ProjectApplicationInfo);
    Console.WriteLine("ProjectFileFormat: " + info.ProjectFileFormat);
}
```

### Zie ook

* class [ProjectFileInfo](../../projectfileinfo/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


