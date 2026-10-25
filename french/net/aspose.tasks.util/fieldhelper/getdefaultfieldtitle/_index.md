---
title: "FieldHelper.GetDefaultFieldTitle"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode FieldHelper. Retourne un titre par défaut du champ spécifique"
type: docs
weight: 10
url: /fr/net/aspose.tasks.util/fieldhelper/getdefaultfieldtitle/
---
## FieldHelper.GetDefaultFieldTitle method

Renvoie un titre par défaut du champ spécifique.

```csharp
public static string GetDefaultFieldTitle(Field field)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| champ | Champ | Champ pour obtenir un titre par défaut. |

### Valeur de retour

Un titre par défaut du champ spécifique si le champ peut être affiché dans la vue de MS Project, sinon null.

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

* enum [Field](../../../aspose.tasks/field/)
* class [FieldHelper](../)
* namespace [Aspose.Tasks.Util](../../fieldhelper/)
* assembly [Aspose.Tasks](../../../)


