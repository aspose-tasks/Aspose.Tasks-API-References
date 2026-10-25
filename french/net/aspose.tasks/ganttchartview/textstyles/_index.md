---
title: "GanttChartView.TextStyles"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété GanttChartView. Obtient ou définit une liste de TextStyle de la vue du diagramme de Gantt"
type: docs
weight: 170
url: /fr/net/aspose.tasks/ganttchartview/textstyles/
---
## GanttChartView.TextStyles property

Obtient ou définit une liste de [`TextStyle`](../../../aspose.tasks.visualization/textstyle/) de la vue du diagramme de Gantt.

```csharp
public List<TextStyle> TextStyles { get; set; }
```

## Exemples

Montre comment lire les styles de texte du diagramme de Gantt.

```csharp
var project = new Project(DataDir + "Project2.mpp");
project.Set(Prj.StatusDate, project.Get(Prj.StartDate));

var view = (GanttChartView)project.Views.ToList()[0];

// itérer sur les styles de texte de la vue du diagramme de Gantt
foreach (var style in view.TextStyles)
{
    Console.WriteLine("Style Item Type: " + style.ItemType);
    Console.WriteLine("Style Font name: " + style.Font.FontFamily);
    Console.WriteLine();
}
```

### Voir aussi

* class [TextStyle](../../../aspose.tasks.visualization/textstyle/)
* class [GanttChartView](../)
* namespace [Aspose.Tasks](../../ganttchartview/)
* assembly [Aspose.Tasks](../../../)


