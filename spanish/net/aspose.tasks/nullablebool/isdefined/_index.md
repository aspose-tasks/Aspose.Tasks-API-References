---
title: "NullableBool.IsDefined"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad NullableBool. Obtiene un valor que indica si el valor fue definido; de lo contrario, false"
type: docs
weight: 20
url: /es/net/aspose.tasks/nullablebool/isdefined/
---
## NullableBool.IsDefined property

Obtiene un valor que indica si el valor fue definido; de lo contrario, false.

```csharp
public bool IsDefined { get; }
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


