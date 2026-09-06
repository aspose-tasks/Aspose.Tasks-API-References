---
title: "XlsxOptions.XlsxOptions"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Constructeur XlsxOptions. Initialise une nouvelle instance de la classe XlsxOptions qui peut être utilisée pour enregistrer le projet au format XLSX"
type: docs
weight: 10
url: /fr/net/aspose.tasks.saving/xlsxoptions/xlsxoptions/
---
## XlsxOptions constructor

Initialise une nouvelle instance de la classe [`XlsxOptions`](../) qui peut être utilisée pour enregistrer le projet au format XLSX.

```csharp
public XlsxOptions()
```

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

* class [XlsxOptions](../)
* namespace [Aspose.Tasks.Saving](../../xlsxoptions/)
* assembly [Aspose.Tasks](../../../)


