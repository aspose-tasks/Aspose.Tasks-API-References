---
title: "Classe XlsxOptions"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Aspose.Tasks.Saving.XlsxOptions class. Permet de spécifier des options supplémentaires lors du rendu des pages de projet en XLSX"
type: docs
weight: 2270
url: /fr/net/aspose.tasks.saving/xlsxoptions/
---
## XlsxOptions class

Permet de spécifier des options supplémentaires lors du rendu des pages de projet au format XLSX.

```csharp
public class XlsxOptions : SimpleSaveOptions
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [XlsxOptions](xlsxoptions/)() | Initialise une nouvelle instance de la classe `XlsxOptions` qui peut être utilisée pour enregistrer le projet au format XLSX. |

## Propriétés

| Nom | Description |
| --- | --- |
| [AssignmentView](../../aspose.tasks.saving/xlsxoptions/assignmentview/) { get; set; } | Obtient ou définit une liste des colonnes de vue des affectations à rendre ([`AssignmentViewColumn`](../../aspose.tasks.visualization/assignmentviewcolumn/)). |
| [Encoding](../../aspose.tasks.saving/xlsxoptions/encoding/) { get; set; } | Obtient ou définit l'encodage du fichier XLSX résultant. La valeur par défaut est UTF8. |
| [ResourceView](../../aspose.tasks.saving/xlsxoptions/resourceview/) { get; set; } | Obtient ou définit une liste des colonnes de vue des ressources à rendre ([`ResourceViewColumn`](../../aspose.tasks.visualization/resourceviewcolumn/)). |
| [SaveFormat](../../aspose.tasks.saving/simplesaveoptions/saveformat/) { get; } | Obtient ou définit le format dans lequel le document sera enregistré si cet objet d'options d'enregistrement est utilisé. |
| [TasksComparer](../../aspose.tasks.saving/simplesaveoptions/taskscomparer/) { get; set; } | Obtient ou définit le comparateur pour trier les tâches sur le diagramme de Gantt et le diagramme de feuille de tâches. |
| [TasksFilter](../../aspose.tasks.saving/simplesaveoptions/tasksfilter/) { get; set; } | Obtient ou définit la condition utilisée pour filtrer les tâches rendues sur les diagrammes Gantt, feuille de tâches et utilisation des tâches. |
| [View](../../aspose.tasks.saving/xlsxoptions/view/) { get; set; } | Obtient ou définit une liste des colonnes de vue ([`GanttChartColumn`](../../aspose.tasks.visualization/ganttchartcolumn/)) à enregistrer au format XLSX. Si non défini, les colonnes par défaut sont enregistrées. |

## Exemples

Montre comment enregistrer un projet dans un fichier XLSX en utilisant les options &lt;see cref=\"P:Aspose.Tasks.Saving.XlsxOptions\"&gt;Days&lt;/see&gt;.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

var options = new XlsxOptions();

// Ajouter les colonnes souhaitées du Gantt Chart
var col = new GanttChartColumn("WBS", 100, delegate(Task task) { return task.Get(Tsk.WBS); });
options.View.Columns.Add(col);

// Ajouter les colonnes souhaitées de la vue des ressources
var rscCol = new ResourceViewColumn("Cost center", 100, delegate(Resource resource) { return resource.Get(Rsc.CostCenter); });
options.ResourceView.Columns.Add(rscCol);

// Ajouter les colonnes souhaitées de la vue des affectations
var assnCol = new AssignmentViewColumn("Notes", 200, delegate(ResourceAssignment assignment) { return assignment.Get(Asn.NotesText); });
options.AssignmentView.Columns.Add(assnCol);

// définir l'encodage
options.Encoding = Encoding.Unicode;

project.Save(OutDir + "UsingXlsxOptions_out.xlsx", options);
```

### Voir aussi

* class [SimpleSaveOptions](../simplesaveoptions/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


