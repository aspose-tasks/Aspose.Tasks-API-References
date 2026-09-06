---
title: "CopyToOptions.CopyToOptions"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Constructeur CopyToOptions. Initialise une nouvelle instance de la classe CopyToOptions"
type: docs
weight: 10
url: /fr/net/aspose.tasks/copytooptions/copytooptions/
---
## CopyToOptions constructor

Initialise une nouvelle instance de la classe [`CopyToOptions`](../).

```csharp
public CopyToOptions()
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


