---
title: "TaskBaseline.Equals"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método TaskBaseline. Devuelve un valor que indica si esta instancia es igual al objeto TaskBaseline especificado."
type: docs
weight: 100
url: /es/net/aspose.tasks/taskbaseline/equals/
---
## Equals(TaskBaseline) {#equals_1}

Devuelve un valor que indica si esta instancia es igual al objeto TaskBaseline especificado.

```csharp
public bool Equals(TaskBaseline other)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| otro | TaskBaseline | el objeto AssignmentBaseline especificado para comparar con esta instancia. |

### Valor devuelto

devuelve true si esta instancia es igual al objeto TaskBaseline especificado; de lo contrario, false.

## Ejemplos

Muestra cómo comprobar la igualdad de líneas base.

```csharp
var project = new Project();

// creando TaskBaseline
var task = project.RootTask.Children.Add("Task");
project.SetBaseline(BaselineType.Baseline);

// mostrar duración de la línea base de la tarea
var baseline1 = task.Baselines.ToList()[0];
var baseline2 = task.Baselines.ToList()[0];

// la igualdad de líneas base se verifica contra los números de la línea base.
Console.WriteLine("Baseline Number 1: " + baseline1.BaselineNumber);
Console.WriteLine("Baseline Number 2: " + baseline2.BaselineNumber);
Console.WriteLine("Are baselines equal: " + baseline1.Equals(baseline2));
```

### Ver también

* class [TaskBaseline](../)
* namespace [Aspose.Tasks](../../taskbaseline/)
* assembly [Aspose.Tasks](../../../)

---

## Equals(object) {#equals_2}

Devuelve un valor que indica si esta instancia es igual a un objeto especificado.

```csharp
public override bool Equals(object obj)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| obj | Objeto | El objeto para comparar con esta instancia. |

### Valor devuelto

**True** if the specified object is a TaskBaseline that has the same UID value as this instance; otherwise, **false**.

## Ejemplos

Muestra cómo comprobar la igualdad de líneas base.

```csharp
var project = new Project();

// creando TaskBaseline
var task = project.RootTask.Children.Add("Task");
project.SetBaseline(BaselineType.Baseline);

// mostrar duración de la línea base de la tarea
var baseline1 = task.Baselines.ToList()[0];
var baseline2 = task.Baselines.ToList()[0];

// la igualdad de líneas base se verifica contra los números de la línea base.
Console.WriteLine("Baseline Number 1: " + baseline1.BaselineNumber);
Console.WriteLine("Baseline Number 2: " + baseline2.BaselineNumber);
Console.WriteLine("Are baselines equal: " + baseline1.Equals(baseline2));
```

### Ver también

* class [TaskBaseline](../)
* namespace [Aspose.Tasks](../../taskbaseline/)
* assembly [Aspose.Tasks](../../../)


