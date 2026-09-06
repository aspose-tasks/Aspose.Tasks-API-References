---
title: "PrimaveraBaseReader.LoadProject"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode PrimaveraBaseReader. Charge le projet avec l'identifiant unique spécifié"
type: docs
weight: 30
url: /fr/net/aspose.tasks/primaverabasereader/loadproject/
---
## PrimaveraBaseReader.LoadProject method

Charge le projet avec l'identifiant unique spécifié.

```csharp
public virtual Project LoadProject(int projectUid)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| projectUid | Int32 | Identifiant unique du projet à charger. |

### Valeur de retour

Projet avec l'identifiant unique spécifié provenant du fichier multi-projets spécifié. Null si le projet n'existe pas.

## Exemples

Montre comment charger un projet à partir d'un fichier XML Primavera lorsque l'uid du projet est connu.

```csharp
var reader = new PrimaveraXmlReader(DataDir + "PrimaveraProject.xml");
var project = reader.LoadProject(3882);
Console.WriteLine(project.Name);
```

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

* class [Project](../../project/)
* class [PrimaveraBaseReader](../)
* namespace [Aspose.Tasks](../../primaverabasereader/)
* assembly [Aspose.Tasks](../../../)


