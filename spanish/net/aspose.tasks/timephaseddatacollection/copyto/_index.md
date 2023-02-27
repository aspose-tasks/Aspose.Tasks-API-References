---
title: TimephasedDataCollection.CopyTo
second_title: Referencia de Aspose.Tasks para la API de .NET
description: TimephasedDataCollection método. Copia los elementos delTimephasedDataCollection a unaArray  a partir de un determinadoArray índice.
type: docs
weight: 90
url: /es/net/aspose.tasks/timephaseddatacollection/copyto/
---
## TimephasedDataCollection.CopyTo method

Copia los elementos del[`TimephasedDataCollection`](../) a unaArray , a partir de un determinadoArray índice.

```csharp
public void CopyTo(TimephasedData[] array, int arrayIndex)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| array | TimephasedData[] | el unidimensionalArray ese es el destino de los elementos copiados de[`TimephasedDataCollection`](../) . ElArray debe tener una indexación basada en cero. |
| arrayIndex | Int32 | El índice de base cero en*array* en el que comienza la copia. |

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentNullException | *array* es nulo. |
| ArgumentOutOfRangeException | *arrayIndex* es menor que 0. |
| ArgumentException | El número de elementos en la fuente.[`TimephasedDataCollection`](../) es mayor que el espacio disponible de*arrayIndex* hasta el final del destino*array* . |

### Ver también

* class [TimephasedData](../../timephaseddata/)
* class [TimephasedDataCollection](../)
* espacio de nombres [Aspose.Tasks](../../timephaseddatacollection/)
* asamblea [Aspose.Tasks](../../../)


