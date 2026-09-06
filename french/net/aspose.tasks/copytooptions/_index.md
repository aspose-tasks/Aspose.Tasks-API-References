---
title: "Classe CopyToOptions"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.CopyToOptions. Permet de spécifier des options supplémentaires lors de la copie des données du projet"
type: docs
weight: 340
url: /fr/net/aspose.tasks/copytooptions/
---
## CopyToOptions class

Permet de spécifier des options supplémentaires lors de la copie des données du projet.

```csharp
public class CopyToOptions
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [CopyToOptions](copytooptions/)() | Initialise une nouvelle instance de la classe `CopyToOptions`. |

## Propriétés

| Nom | Description |
| --- | --- |
| [CopyViewData](../../aspose.tasks/copytooptions/copyviewdata/) { get; set; } | Obtient ou définit une valeur indiquant s'il faut copier les données de vue lors de la copie des données du projet. La valeur par défaut est true. |

## Exemples

Montre comment utiliser les options de copie du projet.

```csharp
var project = new Project(DataDir + "CopyToProjectEmpty.xml");
File.Copy(DataDir + "CopyToProjectEmpty.mpp", OutDir + "ProjectCopying_out.mpp", true);

var mppProject = new Project(OutDir + "ProjectCopying_out.mpp");

// ignorer la copie des données de vue lors de la copie des données communes du projet.
var copyToOptions = new CopyToOptions();
copyToOptions.CopyViewData = false;
project.CopyTo(mppProject, copyToOptions);
```

### Voir aussi

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


