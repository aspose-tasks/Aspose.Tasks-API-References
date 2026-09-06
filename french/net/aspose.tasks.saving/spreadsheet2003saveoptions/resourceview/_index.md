---
title: "Spreadsheet2003SaveOptions.ResourceView"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété Spreadsheet2003SaveOptions. Obtient ou définit une liste des colonnes de vue des ressources à rendre ResourceViewColumn"
type: docs
weight: 30
url: /fr/net/aspose.tasks.saving/spreadsheet2003saveoptions/resourceview/
---
## Spreadsheet2003SaveOptions.ResourceView property

Obtient ou définit une liste des colonnes de vue des ressources à rendre ([`ResourceViewColumn`](../../../aspose.tasks.visualization/resourceviewcolumn/)).

```csharp
public ProjectView ResourceView { get; set; }
```

## Exemples

Montre comment ajouter des colonnes à exporter lors de l'exportation d'un projet au format Spreadsheet2003.

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
* class [Spreadsheet2003SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../spreadsheet2003saveoptions/)
* assembly [Aspose.Tasks](../../../)


