---
title: "NullableBool.Value"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad NullableBool. Obtiene o establece un valor que indica si el valor actual es verdadero o falso"
type: docs
weight: 30
url: /es/net/aspose.tasks/nullablebool/value/
---
## NullableBool.Value property

Obtiene o establece un valor que indica si el valor actual es true o false.

```csharp
public bool Value { get; set; }
```

## Ejemplos

Muestra cómo trabajar con la clase &lt;see cref=\"NullableBool\" /&gt;.

```csharp
var project = new Project();

// Veamos dónde se usa la clase <see cref=\"Aspose.Tasks.NullableBool\" />.
// La principal ventaja de <see cref=\"Aspose.Tasks.NullableBool\" /> es que 
// Se puede establecer como indefinido mediante la construcción
var actualsInSync = new NullableBool(false, false);
Console.WriteLine("'ActualsInSync' Value: " + actualsInSync.Value);
Console.WriteLine("'ActualsInSync' Is Defined: " + actualsInSync.IsDefined);

// ...
// usar instancia de nullable bool
project.Set(Prj.ActualsInSync, actualsInSync);

// ...
var honorConstraints = new NullableBool(true);
Console.WriteLine("'HonorConstraints' ToString: " + honorConstraints.ToString());

// ...
// usar instancia de nullable bool
project.Set(Prj.HonorConstraints, honorConstraints);

// ...
```

### Ver también

* struct [NullableBool](../)
* namespace [Aspose.Tasks](../../nullablebool/)
* assembly [Aspose.Tasks](../../../)


