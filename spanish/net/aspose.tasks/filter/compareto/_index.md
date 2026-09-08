---
title: "Filter.CompareTo"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método Filter. Compara esta instancia con la instancia especificada de la clase Filter y devuelve una indicación de su orden relativo"
type: docs
weight: 90
url: /es/net/aspose.tasks/filter/compareto/
---
## Filter.CompareTo method

Compara esta instancia con la instancia especificada de la clase [`Filter`](../) y devuelve una indicación de su orden relativo.

```csharp
public int CompareTo(Filter other)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| other | Filter | la instancia especificada de la clase [`Filter`](../) para comparar con este objeto. |

### Valor devuelto

una indicación de su orden relativo.

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


