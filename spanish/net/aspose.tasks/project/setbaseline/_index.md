---
title: "Project.SetBaseline"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método de Project. Guarda los campos de línea base en la línea base especificada para todo el proyecto"
type: docs
weight: 1250
url: /es/net/aspose.tasks/project/setbaseline/
---
## SetBaseline(BaselineType) {#setbaseline}

Guarda los campos de línea base en la línea base especificada para todo el proyecto.

```csharp
public void SetBaseline(BaselineType baselineType)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| baselineType | BaselineType | El tipo de línea base donde se guardarán los datos de línea base. |

## Ejemplos

Muestra cómo crear líneas base para todo un proyecto.

```csharp
var project = new Project();

// Agregar tareas
project.RootTask.Children.Add("Task");
project.RootTask.Children.Add("Task2");

// Establecer línea base para tareas especificadas
project.SetBaseline(BaselineType.Baseline);
```

### Ver también

* enum [BaselineType](../../baselinetype/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## SetBaseline(BaselineType, IEnumerable&lt;Task&gt;) {#setbaseline_1}

Guarda los campos de línea base en la línea base especificada para las tareas seleccionadas.

```csharp
public void SetBaseline(BaselineType baselineType, IEnumerable<Task> taskCollection)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| baselineType | BaselineType | El tipo de línea base donde se guardarán los datos de línea base. |
| taskCollection | IEnumerable`1 | Lista de tareas para las que se guardarán los datos de línea base. |

## Ejemplos

Muestra cómo establecer líneas base para tareas específicas.

```csharp
var project = new Project();

// Agregar tareas
var task = project.RootTask.Children.Add("Task");
var task2 = project.RootTask.Children.Add("Task2");

// Establecer línea base para tareas especificadas
project.SetBaseline(BaselineType.Baseline, new[] { task, task2 });
```

### Ver también

* enum [BaselineType](../../baselinetype/)
* class [Task](../../task/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


