---
title: "Énumération PresentationFormat"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Énumération Aspose.Tasks.Visualization.PresentationFormat. Énumération du format de présentation"
type: docs
weight: 3270
url: /fr/net/aspose.tasks.visualization/presentationformat/
---
## PresentationFormat enumeration

Énumération pour le format de présentation.

```csharp
public enum PresentationFormat
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| GanttChart | `0` | Format de présentation du diagramme de Gantt. |
| TaskUsage | `1` | Format de présentation de l'utilisation des tâches. |
| ResourceUsage | `2` | Format de présentation de l'utilisation des ressources. |
| ResourceSheet | `3` | Format de présentation de la feuille de ressources. |
| TaskSheet | `4` | Format de présentation de la feuille de tâches. |

## Exemples

Montre comment rendre la vue de la feuille de ressources.

```csharp
var project = new Project(DataDir + "ResourceSheetView.mpp");

SaveOptions options = new PdfSaveOptions();

// Définir le format de présentation sur Feuille de ressources
options.PresentationFormat = PresentationFormat.ResourceSheet;
project.Save(OutDir + "ResourceSheetView_out.pdf", options);
```

### Voir aussi

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


