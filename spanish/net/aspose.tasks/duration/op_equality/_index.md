---
title: "Duration.op_Equality"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método Duration. Devuelve un valor que indica si esta instancia es igual a un objeto especificado"
type: docs
weight: 140
url: /es/net/aspose.tasks/duration/op_equality/
---
## Duration Equality operator

Devuelve un valor que indica si esta instancia es igual a un objeto especificado.

```csharp
public static bool operator ==(Duration a, Duration b)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| a | Duración | La primera duración. |
| b | Duración | La segunda duración. |

### Valor devuelto

un valor que indica si esta instancia es igual a un objeto especificado

## Ejemplos

Muestra cómo comprobar la igualdad de duraciones.

```csharp
var project = new Project();

var duration1 = project.GetDuration(1, TimeUnitType.Day);
var duration2 = project.GetDuration(1, TimeUnitType.Day);
var duration3 = project.GetDuration(1, TimeUnitType.Hour);

// la igualdad de la duración se verifica contra el timespan subyacente
Console.WriteLine("Duration 1: " + duration1.TimeSpan);
Console.WriteLine("Duration 2: " + duration2.TimeSpan);
Console.WriteLine("Duration 3: " + duration3.TimeSpan);
Console.WriteLine("Are durations 1 and 2 equal: " + duration1.Equals(duration2));
Console.WriteLine("Are durations 1 and 3 equal: " + duration1.Equals(duration3));
```

### Ver también

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


