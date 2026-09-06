---
title: "Class TaskTextStyleEventArgs"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Aspose.Tasks.Visualization.TaskTextStyleEventArgs class. Cette classe représente un ensemble de données liées au rendu du contenu des cellules de tableau."
type: docs
weight: 3390
url: /fr/net/aspose.tasks.visualization/tasktextstyleeventargs/
---
## TaskTextStyleEventArgs class

Cette classe représente un ensemble de données liées au rendu du contenu des cellules de tableau.

```csharp
public class TaskTextStyleEventArgs
```

## Propriétés

| Nom | Description |
| --- | --- |
| [CellTextStyle](../../aspose.tasks.visualization/tasktextstyleeventargs/celltextstyle/) { get; set; } | Obtient ou définit TextStyle qui sera utilisé pour dessiner le contenu de la cellule. Cet objet peut être utilisé pour personnaliser l'apparence d'une cellule de tableau. |
| [Column](../../aspose.tasks.visualization/tasktextstyleeventargs/column/) { get; } | Obtient [`ViewColumn`](../viewcolumn/) à laquelle appartient la cellule actuellement rendue. |
| [Task](../../aspose.tasks.visualization/tasktextstyleeventargs/task/) { get; } | Obtient [`Task`](./task/) qui correspond à la ligne actuellement rendue. |

## Exemples

Montre comment ajouter des colonnes de vue à exporter.

```csharp
public void WorkWithViewColumn()
{
    var project = new Project(DataDir + "Project2.mpp");

    var options = new PdfSaveOptions();
    var columns = new List<ViewColumn>
    {
        new ResourceViewColumn(100, Field.ResourceName),
        new ResourceViewColumn(100, Field.ResourceActualWork),
        new ResourceViewColumn(100, Field.ResourceCost)
    };

    columns[0].TextStyleModificationCallback = new MyTextStyleCallback();

    // itérer sur les colonnes
    foreach (var column in columns)
    {
        Console.WriteLine("Column Name: " + column.Name);
        Console.WriteLine("Column Field: " + column.Field);
        Console.WriteLine("Column Width: " + column.Width);
        Console.WriteLine("Column Callback: " + column.TextStyleModificationCallback);
        Console.WriteLine();
    }

    options.View = new ProjectView(columns);
    options.PresentationFormat = PresentationFormat.ResourceUsage;

    project.Save(OutDir + "WorkWithViewColumn_out.pdf", options);
}

private class MyTextStyleCallback : ITextStyleModificationCallback
{
    /// <summary>
    /// La méthode à appeler avant le rendu d'une cellule de tableau pour une ligne de tâche dans les vues suivantes :
    /// 'Gantt Chart', 'Task Sheet', 'Task Usage'.
    /// </summary>
    /// <param name="args">L'<see cref="T:Aspose.Tasks.Visualization.TaskTextStyleEventArgs" /> objet.</param>
    public void BeforeTaskTextStyleApplied(TaskTextStyleEventArgs args)
    {
        if (args.Task.Get(Tsk.Uid) % 2 == 0)
        {
            args.CellTextStyle.BackgroundColor = 
                args.Column.StringAlignment == HorizontalStringAlignment.Center 
                ? Color.Cyan : Color.Red;
            args.CellTextStyle.BackgroundPattern = BackgroundPattern.SolidFill;
        }
        else
        {
            args.CellTextStyle.Color = Color.DarkGreen;
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


