---
title: "NullableBool.ToString"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método NullableBool. Devuelve una cadena que representa el objeto actual."
type: docs
weight: 60
url: /es/net/aspose.tasks/nullablebool/tostring/
---
## NullableBool.ToString method

Devuelve una cadena que representa el objeto actual.

```csharp
public override string ToString()
```

### Valor devuelto

Una cadena que representa el objeto actual.

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


