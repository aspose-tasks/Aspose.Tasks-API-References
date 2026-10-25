---
title: "Duration.Equals"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método Duration. Devuelve un valor que indica si esta instancia es igual a un objeto especificado"
type: docs
weight: 80
url: /es/net/aspose.tasks/duration/equals/
---
## Equals(Duration) {#equals}

Devuelve un valor que indica si esta instancia es igual a un objeto especificado.

```csharp
public bool Equals(Duration other)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| otro | Duración | El objeto para comparar con esta instancia. |

### Valor devuelto

Devuelve **True** si otra instancia de Duration tiene los mismos valores de TimeSpan y TimeUnit que esta instancia; de lo contrario, **false**.

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

---

## Equals(object) {#equals_1}

Devuelve un valor que indica si esta instancia es igual a un objeto especificado.

```csharp
public override bool Equals(object obj)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| obj | Objeto | El objeto para comparar con esta instancia. |

### Valor devuelto

**True** if the specified object is a Duration that has the same TimeSpan and TimeUnit values as this instance; otherwise, **false**.

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


