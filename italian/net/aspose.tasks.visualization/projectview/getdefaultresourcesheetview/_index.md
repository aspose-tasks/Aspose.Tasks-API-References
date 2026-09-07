---
title: "ProjectView.GetDefaultResourceSheetView"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo ProjectView. Include le colonne di risorsa Uid, nome, tipo, materiale, etichetta, iniziali, gruppo, unità massime, tariffa standard, tariffa straordinaria, costo per utilizzo, accumulato, calendario base e codice"
type: docs
weight: 40
url: /it/net/aspose.tasks.visualization/projectview/getdefaultresourcesheetview/
---
## ProjectView.GetDefaultResourceSheetView method

Include le colonne Uid, nome risorsa, tipo, etichetta materiale, iniziali, gruppo, unità massime, tariffa standard, tariffa straordinaria, costo per utilizzo, accumulo a, calendario base e codice risorsa.

```csharp
public static ProjectView GetDefaultResourceSheetView()
```

### Valore di ritorno

una vista che contiene un elenco di [`ResourceViewColumn`](../../resourceviewcolumn/).

## Esempi

Mostra come salvare un progetto con la vista del foglio risorse.

```csharp
var project = new Project(DataDir + "Project2.mpp");
SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.Months,
    View = ProjectView.GetDefaultResourceSheetView()
};

project.Save(OutDir + "WorkWithProjectView_ResourceSheetView_out.pdf", options);
```

### Vedi anche

* class [ProjectView](../)
* namespace [Aspose.Tasks.Visualization](../../projectview/)
* assembly [Aspose.Tasks](../../../)


