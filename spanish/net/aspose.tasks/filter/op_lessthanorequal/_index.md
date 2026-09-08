---
title: "Filter.op_LessThanOrEqual"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método Filter. Devuelve un valor que indica si esta instancia es menor o igual que un objeto especificado"
type: docs
weight: 170
url: /es/net/aspose.tasks/filter/op_lessthanorequal/
---
## Filter LessThanOrEqual operator

Devuelve un valor que indica si esta instancia es menor o igual que un objeto especificado.

```csharp
public static bool operator <=(Filter a, Filter b)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| a | Filter | El primer filtro. |
| b | Filter | El segundo filtro. |

### Valor devuelto

un valor que indica si esta instancia es menor o igual que un objeto especificado

## Ejemplos

Muestra cómo comprobar la igualdad del filtro.

```csharp
var project = new Project(DataDir + "ReadFilterDefinitionData.mpp");
List<Filter> filters = project.TaskFilters.ToList();

var filter1 = filters[0];
var filter2 = filters[1];

// la igualdad de los filtros se verifica contra el UID del filtro.
Console.WriteLine("Filter 1 UID: " + filter1.Uid);
Console.WriteLine("Filter 2 UID: " + filter2.Uid);
Console.WriteLine("Are filters equal: " + filter1.Equals(filter2));
```

### Ver también

* class [Filter](../)
* namespace [Aspose.Tasks](../../filter/)
* assembly [Aspose.Tasks](../../../)


