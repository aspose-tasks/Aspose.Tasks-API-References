---
title: "SaveOptions.CustomPageSize"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété SaveOptions. Obtient ou définit la taille de page personnalisée en points (1 point = 1/72 de pouce)."
type: docs
weight: 20
url: /fr/net/aspose.tasks.saving/saveoptions/custompagesize/
---
## SaveOptions.CustomPageSize property

Obtient ou définit la taille de page personnalisée en points (1 point = 1/72 de pouce).

```csharp
public SizeF CustomPageSize { get; set; }
```

## Exemples

Montre comment définir la taille de page personnalisée lorsque le projet est enregistré en PDF.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions();
options.PresentationFormat = PresentationFormat.GanttChart;
options.CustomPageSize = new SizeF(5.8F * 72, 8.3F * 72);

project.Save(OutDir + "WorkWithCustomPageSize_out.pdf", options);
```

### Voir aussi

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


