---
title: "XlsxOptions.Encoding"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad XlsxOptions. Obtiene o establece la codificación del archivo XLSX resultante. El valor predeterminado es UTF8"
type: docs
weight: 30
url: /es/net/aspose.tasks.saving/xlsxoptions/encoding/
---
## XlsxOptions.Encoding property

Obtiene o establece la codificación del archivo XLSX resultante. El valor predeterminado es UTF8.

```csharp
public Encoding Encoding { get; set; }
```

## Ejemplos

Muestra cómo guardar un proyecto en un archivo XLSX usando las opciones &lt;see cref=\"P:Aspose.Tasks.Saving.XlsxOptions\"&gt;Days&lt;/see&gt;.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

var options = new XlsxOptions();

// Agregar columnas deseadas del diagrama Gantt
var col = new GanttChartColumn("WBS", 100, delegate(Task task) { return task.Get(Tsk.WBS); });
options.View.Columns.Add(col);

// Agregar columnas deseadas de la vista de recursos
var rscCol = new ResourceViewColumn("Cost center", 100, delegate(Resource resource) { return resource.Get(Rsc.CostCenter); });
options.ResourceView.Columns.Add(rscCol);

// Agregar columnas deseadas de la vista de asignaciones
var assnCol = new AssignmentViewColumn("Notes", 200, delegate(ResourceAssignment assignment) { return assignment.Get(Asn.NotesText); });
options.AssignmentView.Columns.Add(assnCol);

// establecer codificación
options.Encoding = Encoding.Unicode;

project.Save(OutDir + "UsingXlsxOptions_out.xlsx", options);
```

### Ver también

* class [XlsxOptions](../)
* namespace [Aspose.Tasks.Saving](../../xlsxoptions/)
* assembly [Aspose.Tasks](../../../)


