---
title: "ProjectView.GetDefaultAssignmentView"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo ProjectView. Include le colonne di assegnazione Uid, nome attività, nome risorsa, lavoro e durata"
type: docs
weight: 20
url: /it/net/aspose.tasks.visualization/projectview/getdefaultassignmentview/
---
## ProjectView.GetDefaultAssignmentView method

Include le colonne Uid, nome attività, nome risorsa, lavoro e durata dell'assegnazione.

```csharp
public static ProjectView GetDefaultAssignmentView()
```

### Valore di ritorno

una vista che contiene un elenco di [`AssignmentViewColumn`](../../assignmentviewcolumn/).

## Esempi

Mostra come salvare un progetto con la visualizzazione delle assegnazioni.

```csharp
var project = new Project(DataDir + "Project2.mpp");
SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.Months,
    View = ProjectView.GetDefaultAssignmentView()
};

project.Save(OutDir + "WorkWithProjectView_AssignmentView_out.pdf", options);
```

### Vedi anche

* class [ProjectView](../)
* namespace [Aspose.Tasks.Visualization](../../projectview/)
* assembly [Aspose.Tasks](../../../)


