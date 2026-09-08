---
title: "MPPSaveOptions.WriteFilters"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad MPPSaveOptions. Obtiene o establece un valor que indica si se deben escribir datos de filtros al guardar un proyecto en formato MPP. Los datos de filtros incluyen las colecciones Project.TaskFilters y Project.ResourceFilters."
type: docs
weight: 50
url: /es/net/aspose.tasks.saving/mppsaveoptions/writefilters/
---
## MPPSaveOptions.WriteFilters property

Obtiene o establece un valor que indica si se deben escribir los datos de filtros al guardar un proyecto en formato MPP. Los datos de filtros incluyen las colecciones Project.TaskFilters y Project.ResourceFilters.

```csharp
public bool WriteFilters { get; set; }
```

## Observaciones

Actualmente compatible con los formatos MSP 2010 o posteriores.

## Ejemplos

Muestra cómo agregar y guardar un nuevo filtro de tareas en un proyecto MPP.

```csharp
Project project = new Project();

project.TaskFilters.Clear();
project.ResourceFilters.Clear();

var filter = new Filter();
filter.Name = "New Task Filter";
filter.FilterType = ItemType.TaskItem;
filter.ShowInMenu = true;
filter.ShowRelatedSummaryRows = true;

filter.Criteria = new FilterCriteria();

var criteria1 = new FilterCriteria();
criteria1.Field = Field.TaskNumber13;
criteria1.Test = FilterComparisonType.IsLessThan;
criteria1.Values[0] = 34.3D;

filter.Criteria.CriteriaRows.Add(criteria1);
project.TaskFilters.Add(filter);

SimpleSaveOptions options = new MPPSaveOptions() { WriteFilters = true };
project.Save(OutDir + "output_new_filter.mpp", options);
```

### Ver también

* class [MPPSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../mppsaveoptions/)
* assembly [Aspose.Tasks](../../../)


