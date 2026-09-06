---
title: "CopyToOptions.CopyViewData"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété CopyToOptions. Obtient ou définit une valeur indiquant s'il faut copier les données de vue lors de la copie des données du projet. La valeur par défaut est true"
type: docs
weight: 20
url: /fr/net/aspose.tasks/copytooptions/copyviewdata/
---
## CopyToOptions.CopyViewData property

Obtient ou définit une valeur indiquant s'il faut copier les données de vue lors de la copie des données du projet. La valeur par défaut est true.

```csharp
public bool CopyViewData { get; set; }
```

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

* class [CopyToOptions](../)
* namespace [Aspose.Tasks](../../copytooptions/)
* assembly [Aspose.Tasks](../../../)


