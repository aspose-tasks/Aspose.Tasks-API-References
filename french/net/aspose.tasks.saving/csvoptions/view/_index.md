---
title: "CsvOptions.View"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété CsvOptions. Obtient ou définit une liste des colonnes d'affichage GanttChartColumn à enregistrer au format XLSX. Si non définies, les colonnes par défaut sont enregistrées"
type: docs
weight: 60
url: /fr/net/aspose.tasks.saving/csvoptions/view/
---
## CsvOptions.View property

Obtient ou définit une liste des colonnes d'affichage ([`GanttChartColumn`](../../../aspose.tasks.visualization/ganttchartcolumn/)) à enregistrer au format XLSX. Si non définies, les colonnes par défaut sont enregistrées.

```csharp
public ProjectView View { get; set; }
```

## Exemples

Montre comment utiliser &lt;see cref=\"Aspose.Tasks.Saving.CsvOptions\" /&gt; pour prendre les colonnes du diagramme de Gantt par défaut et

```csharp
// enregistrez-les dans un fichier CSV.
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

CsvOptions options = new CsvOptions();
options.TextDelimiter = CsvTextDelimiter.Tab;

var view = project.DefaultView;
options.View = ProjectView.GetDefaultGanttChartView();
options.View.Columns.Clear();

foreach (var t in view.Table.TableFields)
{
    var columnTitle = string.IsNullOrEmpty(t.Title) ? FieldHelper.GetDefaultFieldTitle(t.Field) : t.Title;
    options.View.Columns.Add(new GanttChartColumn(columnTitle, 10, t.Field));
}

project.Save(OutDir + "CustomizeViewForCsvOptions_out.csv", options);
```

### Voir aussi

* class [ProjectView](../../../aspose.tasks.visualization/projectview/)
* class [CsvOptions](../)
* namespace [Aspose.Tasks.Saving](../../csvoptions/)
* assembly [Aspose.Tasks](../../../)


