---
title: "Filter.Equals"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método Filter. Devuelve un valor que indica si esta instancia es igual al objeto AssignmentBaseline especificado."
type: docs
weight: 100
url: /es/net/aspose.tasks/filter/equals/
---
## Equals(Filter) {#equals}

Devuelve un valor que indica si esta instancia es igual al objeto AssignmentBaseline especificado.

```csharp
public bool Equals(Filter other)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| otro | Filter | el objeto AssignmentBaseline especificado para comparar con esta instancia. |

### Valor devuelto

devuelve true si esta instancia es igual al objeto AssignmentBaseline especificado; de lo contrario, false.

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

---

## Equals(object) {#equals_1}

Devuelve un valor que indica si esta instancia es igual al objeto AssignmentBaseline especificado.

```csharp
public override bool Equals(object obj)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| obj | Objeto | el objeto AssignmentBaseline especificado para comparar con esta instancia. |

### Valor devuelto

devuelve true si esta instancia es igual al objeto AssignmentBaseline especificado; de lo contrario, false.

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


