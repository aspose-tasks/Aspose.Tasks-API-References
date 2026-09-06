---
title: "Classe GanttChartColumn"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.Visualization.GanttChartColumn. Classe de vue des projets"
type: docs
weight: 3090
url: /fr/net/aspose.tasks.visualization/ganttchartcolumn/
---
## GanttChartColumn class

Classe de vue du projet

```csharp
public sealed class GanttChartColumn : ViewColumn
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [GanttChartColumn](ganttchartcolumn/#constructor)(int, Field) | Initialise une nouvelle instance de la classe GanttChartColumn. |
| [GanttChartColumn](ganttchartcolumn/#constructor_1)(string, int, Field) | Initialise une nouvelle instance de la classe GanttChartColumn. |
| [GanttChartColumn](ganttchartcolumn/#constructor_2)(string, int, TaskToColumnTextConverter) | Initialise une nouvelle instance de la classe GanttChartColumn. |
| [GanttChartColumn](ganttchartcolumn/#constructor_3)(string, int, TaskToColumnTextConverter, Field) | Initialise une nouvelle instance de la classe GanttChartColumn. |

## Propriétés

| Nom | Description |
| --- | --- |
| override [Field](../../aspose.tasks.visualization/ganttchartcolumn/field/) { get; set; } | Champ de colonne. [`Field`](./field/). |
| [Name](../../aspose.tasks.visualization/viewcolumn/name/) { get; } | Obtient le nom de la colonne. |
| [StringAlignment](../../aspose.tasks.visualization/viewcolumn/stringalignment/) { get; set; } | Obtient ou définit l'alignement du texte (peut être l'une des valeurs de l'énumération [`HorizontalStringAlignment`](../horizontalstringalignment/)). |
| [TextStyleModificationCallback](../../aspose.tasks.visualization/viewcolumn/textstylemodificationcallback/) { get; set; } | Obtient ou définit le rappel qui peut être utilisé pour personnaliser l'apparence des cellules de la colonne. |
| [Width](../../aspose.tasks.visualization/viewcolumn/width/) { get; } | Obtient la largeur de la colonne. |

## Méthodes

| Nom | Description |
| --- | --- |
| [GetColumnText](../../aspose.tasks.visualization/ganttchartcolumn/getcolumntext/)(Task) | Convertit la tâche actuelle en texte de colonne. |

## Exemples

Montre comment ajouter des colonnes de vue du diagramme de Gantt à exporter.

```csharp
var project = new Project(DataDir + "Project2.mpp");
var task = project.RootTask.Children.GetById(1);

var columns = new List<ViewColumn>
{
    new GanttChartColumn(20, Field.TaskUniqueID),
    new GanttChartColumn("Name", 150, Field.TaskName),
    new GanttChartColumn("Start", 100, Field.TaskStart),
    new GanttChartColumn("End", 100, Field.TaskFinish),
    new GanttChartColumn("R-Initials", 100, Field.TaskResourceInitials),
    new GanttChartColumn("R-Names", 100, Field.TaskResourceNames),
    new GanttChartColumn("Work", 50, Field.TaskWork),
    new GanttChartColumn(
        "Cost", 
        80,
        delegate(Task t)
        {
            return t.Get(Tsk.Cost).ToString(CultureInfo.InvariantCulture);
        }),
    new GanttChartColumn(
        "Actual Cost", 
        80,
        delegate(Task t)
        {
            return t.Get(Tsk.ActualCost).ToString(CultureInfo.InvariantCulture);
        },
        Field.TaskActualCost)
};

// itérer sur les colonnes
foreach (var column in columns)
{
    var col = (GanttChartColumn)column;
    Console.WriteLine("Column Name: " + col.Name);
    Console.WriteLine("Column Field: " + col.Field);
    Console.WriteLine("Column Text: " + col.GetColumnText(task));
    Console.WriteLine();
}

var options = new CsvOptions
{
    View = new ProjectView(columns)
};

project.Save(OutDir + "WorkWithGanttChartColumn_out.csv", options);
```

### Voir aussi

* class [ViewColumn](../viewcolumn/)
* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


