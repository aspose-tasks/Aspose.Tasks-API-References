---
title: "PrimaveraXmlReader.PrimaveraXmlReader"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Constructeur PrimaveraXmlReader. Initialise une nouvelle instance de la classe PrimaveraXmlReader"
type: docs
weight: 10
url: /fr/net/aspose.tasks/primaveraxmlreader/primaveraxmlreader/
---
## PrimaveraXmlReader(string) {#constructor_1}

Initialise une nouvelle instance de la classe [`PrimaveraXmlReader`](../).

```csharp
public PrimaveraXmlReader(string templatePath)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| templatePath | Chaîne | Chemin vers le modèle où le projet ou les projets Primavera Xml sont situés |

## Exemples

Montre comment examiner les informations des projets courts à partir d'un fichier Primavera XML.

```csharp
var reader = new PrimaveraXmlReader(DataDir + "MultiprojectWithExternal.xml");
var projectInfos = reader.GetProjectInfos();
foreach (var info in projectInfos)
{
    Console.WriteLine("{0} - '{1}' - {2}", info.Uid, info.Name, info.ExportFlag);
}
```

### Voir aussi

* class [PrimaveraXmlReader](../)
* namespace [Aspose.Tasks](../../primaveraxmlreader/)
* assembly [Aspose.Tasks](../../../)

---

## PrimaveraXmlReader(Stream) {#constructor}

Initialise une nouvelle instance de la classe [`PrimaveraXmlReader`](../).

```csharp
public PrimaveraXmlReader(Stream stream)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| flux | Flux | Flux contenant le contenu Primavera Xml. |

## Exemples

Montre comment importer un projet à partir d'un flux Primavera XML.

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

### Voir aussi

* class [PrimaveraXmlReader](../)
* namespace [Aspose.Tasks](../../primaveraxmlreader/)
* assembly [Aspose.Tasks](../../../)


