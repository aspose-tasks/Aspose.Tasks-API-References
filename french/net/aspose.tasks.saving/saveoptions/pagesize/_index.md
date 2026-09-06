---
title: "SaveOptions.PageSize"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété SaveOptions. Obtient ou définit la taille de la page à rendre. La valeur par défaut est PageSize.A4"
type: docs
weight: 130
url: /fr/net/aspose.tasks.saving/saveoptions/pagesize/
---
## SaveOptions.PageSize property

Obtient ou définit la taille de la page à rendre (la valeur par défaut est PageSize.A4).

```csharp
public PageSize PageSize { get; set; }
```

## Exemples

Montre comment définir la taille de la page (peut être l'une des valeurs de l'énumération &lt;see cref="P:Aspose.Tasks.Visualization.TiffCompression" /&gt;).

```csharp
var project = new Project(DataDir + "Project2.mpp");

const PresentationFormat format = PresentationFormat.GanttChart;

// Rendre le projet à toutes les tailles de page prédéfinies
foreach (var pageSize in (PageSize[])Enum.GetValues(typeof(PageSize)))
{
    var options = new PdfSaveOptions
    {
        PresentationFormat = format,
        FitContent = true,
        PageSize = pageSize
    };
    project.Save(OutDir + "PredefinedPageSizes_" + format + "_" + pageSize + "_out.pdf", options);
}
```

### Voir aussi

* enum [PageSize](../../../aspose.tasks.visualization/pagesize/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


