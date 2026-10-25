---
title: "Duration.GetHashCode"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método Duration. Devuelve un valor de código hash para este objeto."
type: docs
weight: 90
url: /es/net/aspose.tasks/duration/gethashcode/
---
## Duration.GetHashCode method

Devuelve un valor de código hash para este objeto.

```csharp
public override int GetHashCode()
```

### Valor devuelto

devuelve un valor de código hash para esta instancia de duración.

## Ejemplos

Muestra cómo obtener un código hash de una duración.

```csharp
var project = new Project();

var duration1 = project.GetDuration(1, TimeUnitType.Day);
var duration2 = project.GetDuration(1, TimeUnitType.Day);
var duration3 = project.GetDuration(1, TimeUnitType.Hour);

// el código hash de un calendario se basa en el tipo de unidad de tiempo y el valor inicial de la duración
// por lo que los siguientes códigos hash son iguales
Console.WriteLine("Duration 1 Hash Code: {0}", duration1.GetHashCode());
Console.WriteLine("Duration 2 Hash Code: {0}", duration2.GetHashCode());
Console.WriteLine("Are duration's hash codes of duration 1 and duration 2 equal: {0}", duration1.GetHashCode().Equals(duration2.GetHashCode()));

// pero los códigos hash de la duración 1 y 3 no lo son
Console.WriteLine("Duration 1 Hash Code: {0}", duration1.GetHashCode());
Console.WriteLine("Duration 3 Hash Code: {0}", duration3.GetHashCode());
Console.WriteLine("Are duration's hash codes of duration 1 and duration 2 equal: {0}", duration1.GetHashCode().Equals(duration3.GetHashCode()));
```

### Ver también

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


