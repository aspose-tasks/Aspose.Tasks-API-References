---
title: "XpsOptions.XpsOptions"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Constructeur XpsOptions. Initialise une nouvelle instance de la classe XpsOptions"
type: docs
weight: 10
url: /fr/net/aspose.tasks.saving/xpsoptions/xpsoptions/
---
## XpsOptions constructor

Initialise une nouvelle instance de la classe [`XpsOptions`](../).

```csharp
public XpsOptions()
```

## Exemples

Montre comment enregistrer le projet en tant que fichier XPS.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// créer des options d'enregistrement XPS et ajuster les paramètres
var options = new XpsOptions
{
    RenderMetafileAsBitmap = true
};

project.Save(OutDir + "UseSvgOptions_out.xps", options);
```

### Voir aussi

* class [XpsOptions](../)
* namespace [Aspose.Tasks.Saving](../../xpsoptions/)
* assembly [Aspose.Tasks](../../../)


