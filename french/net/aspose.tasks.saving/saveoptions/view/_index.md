---
title: "SaveOptions.View"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété SaveOptions. Obtient ou définit une liste des colonnes de vue à rendre GanttChartColumn. Si non définie, seuls les identifiants de tâche, les noms de tâche, le début et la fin sont rendus. Si les propriétés View et ViewSettings sont toutes deux définies, les colonnes de View remplacent les colonnes de ViewSettings."
type: docs
weight: 230
url: /fr/net/aspose.tasks.saving/saveoptions/view/
---
## SaveOptions.View property

Obtient ou définit une liste des colonnes de vue à rendre ([`GanttChartColumn`](../../../aspose.tasks.visualization/ganttchartcolumn/)). Si non définie, seuls les identifiants de tâche, les noms de tâche, le début et la fin sont rendus. Si les propriétés View et [`ViewSettings`](../viewsettings/) sont toutes deux définies, les colonnes de View remplacent les colonnes de ViewSettings.

```csharp
public ProjectView View { get; set; }
```

## Exemples

Montre comment ajouter des colonnes de vue à exporter lors de l'exportation du projet.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

var options = new Spreadsheet2003SaveOptions();
var ganttChartColumn = new GanttChartColumn("WBS", 100, delegate(Task task) { return task.Get(Tsk.WBS); });
options.View.Columns.Add(ganttChartColumn);

var resourceViewColumn = new ResourceViewColumn("Cost center", 100, delegate(Resource resource) { return resource.Get(Rsc.CostCenter); });
options.ResourceView.Columns.Add(resourceViewColumn);

var assignmentViewColumn = new AssignmentViewColumn("Notes", 200, delegate(ResourceAssignment assignment) { return assignment.Get(Asn.NotesText); });
options.AssignmentView.Columns.Add(assignmentViewColumn);

project.Save(OutDir + "UsingSpreadsheet2003SaveOptions_out.xml", options);
```

### Voir aussi

* class [ProjectView](../../../aspose.tasks.visualization/projectview/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


