---
title: "Project.Set"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método de Project. Asocia la propiedad especificada al valor especificado en este contenedor"
type: docs
weight: 1240
url: /es/net/aspose.tasks/project/set/
---
## Set&lt;T&gt;(Key&lt;T, PrjKey&gt;, T) {#set_1}

Mapea la propiedad especificada al valor especificado en este contenedor.

```csharp
public void Set<T>(Key<T, PrjKey> key, T val)
```

| Parámetro | Descripción |
| --- | --- |
| T | el tipo del valor asignado. |
| key | la clave de propiedad especificada. [`Prj`](../../prj/) para obtener la clave de la propiedad. |
| valor | el valor. |

## Ejemplos

Muestra cómo establecer los atributos de la tarea.

```csharp
var project = new Project();
project.Set(Prj.NewTaskStartDate, TaskStartDateType.CurrentDate);
project.Save(OutDir + "SetAttributesForNewTasks_out.xml", SaveFileFormat.Xml);
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Set(Key&lt;DateTime, PrjKey&gt;, DateTime) {#set}

Mapea la propiedad especificada al valor especificado en este contenedor.

```csharp
public void Set(Key<DateTime, PrjKey> key, DateTime val)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| key | Key`2 | la clave de propiedad especificada. [`Prj`](../../prj/) para obtener la clave de la propiedad. |
| valor | DateTime | el valor. |

## Ejemplos

Muestra cómo establecer los atributos de la tarea.

```csharp
var project = new Project();
project.Set(Prj.NewTaskStartDate, TaskStartDateType.CurrentDate);
project.Save(OutDir + "SetAttributesForNewTasks_out.xml", SaveFileFormat.Xml);
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


