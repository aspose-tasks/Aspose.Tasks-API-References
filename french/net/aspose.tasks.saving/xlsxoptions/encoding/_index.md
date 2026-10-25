---
title: "XlsxOptions.Encoding"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété XlsxOptions. Obtient ou définit l'encodage du fichier XLSX résultant. La valeur par défaut est UTF8"
type: docs
weight: 30
url: /fr/net/aspose.tasks.saving/xlsxoptions/encoding/
---
## XlsxOptions.Encoding property

Obtient ou définit l'encodage du fichier XLSX résultant. La valeur par défaut est UTF8.

```csharp
public Encoding Encoding { get; set; }
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


