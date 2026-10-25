---
title: "Classe CsvOptions"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Aspose.Tasks.Saving.CsvOptions class. Permet de spécifier des options supplémentaires lors de l'enregistrement du projet au format CSV"
type: docs
weight: 1980
url: /fr/net/aspose.tasks.saving/csvoptions/
---
## CsvOptions class

Permet de spécifier des options supplémentaires lors de l'enregistrement du projet au format CSV.

```csharp
public class CsvOptions : SimpleSaveOptions
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [CsvOptions](csvoptions/)() | Initialise une nouvelle instance de la classe `CsvOptions` qui peut être utilisée pour enregistrer le projet au format CSV. |

## Propriétés

| Nom | Description |
| --- | --- |
| [DataCategory](../../aspose.tasks.saving/csvoptions/datacategory/) { get; set; } | Obtient ou définit une catégorie de données à enregistrer. |
| [Encoding](../../aspose.tasks.saving/csvoptions/encoding/) { get; set; } | Obtient ou définit un encodage avec lequel enregistrer le CSV. |
| [IncludeHeaders](../../aspose.tasks.saving/csvoptions/includeheaders/) { get; set; } | Obtient ou définit une valeur indiquant s'il faut inclure les en-têtes ou non (la valeur par défaut est TRUE). |
| [SaveFormat](../../aspose.tasks.saving/simplesaveoptions/saveformat/) { get; } | Obtient ou définit le format dans lequel le document sera enregistré si cet objet d'options d'enregistrement est utilisé. |
| [TasksComparer](../../aspose.tasks.saving/simplesaveoptions/taskscomparer/) { get; set; } | Obtient ou définit le comparateur pour trier les tâches sur le diagramme de Gantt et le diagramme de feuille de tâches. |
| [TasksFilter](../../aspose.tasks.saving/simplesaveoptions/tasksfilter/) { get; set; } | Obtient ou définit la condition utilisée pour filtrer les tâches rendues sur les diagrammes Gantt, feuille de tâches et utilisation des tâches. |
| [TextDelimiter](../../aspose.tasks.saving/csvoptions/textdelimiter/) { get; set; } | Obtient ou définit un délimiteur de texte. |
| [View](../../aspose.tasks.saving/csvoptions/view/) { get; set; } | Obtient ou définit une liste des colonnes de vue ([`GanttChartColumn`](../../aspose.tasks.visualization/ganttchartcolumn/)) à enregistrer au format XLSX. Si non défini, les colonnes par défaut sont enregistrées. |

## Exemples

Montre comment utiliser &lt;see cref=\"Aspose.Tasks.Saving.CsvOptions\" /&gt; pour enregistrer un projet au format CSV.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");
var options = new CsvOptions
{
    DataCategory = DataCategory.Resources,
    TextDelimiter = CsvTextDelimiter.Semicolon,
    Encoding = Encoding.Unicode, IncludeHeaders = true
};

project.Save(OutDir + "WorkWithCsvOptions_out.csv", options);
```

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

* class [SimpleSaveOptions](../simplesaveoptions/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


