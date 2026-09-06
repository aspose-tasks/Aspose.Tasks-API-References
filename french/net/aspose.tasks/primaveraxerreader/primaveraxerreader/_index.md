---
title: "PrimaveraXerReader.PrimaveraXerReader"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Constructeur PrimaveraXerReader. Initialise une nouvelle instance de la classe PrimaveraXerReader"
type: docs
weight: 10
url: /fr/net/aspose.tasks/primaveraxerreader/primaveraxerreader/
---
## PrimaveraXerReader(string) {#constructor_1}

Initialise une nouvelle instance de la classe [`PrimaveraXerReader`](../).

```csharp
public PrimaveraXerReader(string xerFilePath)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| xerFilePath | Chaîne | Chemin vers le fichier .xer où le projet ou les projets Primavera sont situés. |

## Exemples

Montre comment examiner les informations des projets courts à partir d'un fichier Primavera XER.

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

### Voir aussi

* class [PrimaveraXerReader](../)
* namespace [Aspose.Tasks](../../primaveraxerreader/)
* assembly [Aspose.Tasks](../../../)

---

## PrimaveraXerReader(Stream) {#constructor}

Initialise une nouvelle instance de la classe [`PrimaveraXerReader`](../).

```csharp
public PrimaveraXerReader(Stream stream)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| flux | Flux | Flux contenant le contenu XER de Primavera. |

### Voir aussi

* class [PrimaveraXerReader](../)
* namespace [Aspose.Tasks](../../primaveraxerreader/)
* assembly [Aspose.Tasks](../../../)


