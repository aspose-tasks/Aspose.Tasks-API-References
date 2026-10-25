---
title: "PrimaveraReadOptions.ProjectUid"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété PrimaveraReadOptions. Obtient ou définit l'UID d'un projet à lire à partir d'un fichier contenant plusieurs projets"
type: docs
weight: 30
url: /fr/net/aspose.tasks/primaverareadoptions/projectuid/
---
## PrimaveraReadOptions.ProjectUid property

Obtient ou définit l'UID d'un projet à lire à partir d'un fichier contenant plusieurs projets.

```csharp
public int ProjectUid { get; set; }
```

## Exemples

Montre comment lire un projet à partir d'un fichier Primavera XML ou Primavera XER contenant plusieurs projets.

```csharp
var options = new PrimaveraReadOptions();
options.ProjectUid = 3881;

// Renvoie le projet avec un UID spécial
var project = new Project(DataDir + "PrimaveraProject.xml", options);
Console.WriteLine(project.Get(Prj.Name));
```

### Voir aussi

* class [PrimaveraReadOptions](../)
* namespace [Aspose.Tasks](../../primaverareadoptions/)
* assembly [Aspose.Tasks](../../../)


