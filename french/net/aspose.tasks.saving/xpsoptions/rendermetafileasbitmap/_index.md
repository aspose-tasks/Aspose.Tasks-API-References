---
title: "XpsOptions.RenderMetafileAsBitmap"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété XpsOptions. Obtient ou définit une valeur indiquant si un métafichier doit être rendu sous forme de bitmap"
type: docs
weight: 20
url: /fr/net/aspose.tasks.saving/xpsoptions/rendermetafileasbitmap/
---
## XpsOptions.RenderMetafileAsBitmap property

Obtient ou définit une valeur indiquant si un métafichier doit être rendu en bitmap.

```csharp
public bool RenderMetafileAsBitmap { get; set; }
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


