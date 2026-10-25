---
title: "Estructura NullableBool"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Aspose.Tasks.NullableBool struct. Una clase para valores booleanos con la posibilidad de comprobar si el valor fue definido o no"
type: docs
weight: 1110
url: /es/net/aspose.tasks/nullablebool/
---
## NullableBool structure

Una clase para valores booleanos con la posibilidad de comprobar si el valor fue definido o no.

```csharp
public struct NullableBool : IEquatable<NullableBool>
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [NullableBool](nullablebool/#constructor)(bool) | Inicializa una nueva instancia de la estructura `NullableBool` con el valor booleano especificado. |
| [NullableBool](nullablebool/#constructor_1)(bool, bool) | Inicializa una nueva instancia de la estructura `NullableBool`. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [IsDefined](../../aspose.tasks/nullablebool/isdefined/) { get; } | Obtiene un valor que indica si el valor fue definido; de lo contrario, false. |
| [Value](../../aspose.tasks/nullablebool/value/) { get; set; } | Obtiene o establece un valor que indica si el valor actual es true o false. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Equals](../../aspose.tasks/nullablebool/equals/#equals)(NullableBool) | Devuelve una bandera que indica si esta instancia es igual a la instancia especificada de la clase `NullableBool`. |
| override [Equals](../../aspose.tasks/nullablebool/equals/#equals_1)(object) | Devuelve una bandera que indica si esta instancia es igual al objeto especificado. |
| override [GetHashCode](../../aspose.tasks/nullablebool/gethashcode/)() | Devuelve un valor de código hash para la instancia de la clase `NullableBool`. |
| override [ToString](../../aspose.tasks/nullablebool/tostring/)() | Devuelve una cadena que representa el objeto actual. |
| [operator ==](../../aspose.tasks/nullablebool/op_equality/) | Devuelve un valor que indica si esta instancia es igual a un objeto especificado. |
| [implicit operator](../../aspose.tasks/nullablebool/op_implicit/#op_implicit_1) | Convierte implícitamente una instancia de `NullableBool` a un valor booleano. Devuelve true cuando [`Value`](./value/) es true y [`IsDefined`](./isdefined/) es true. (2 operadores) |
| [operator !=](../../aspose.tasks/nullablebool/op_inequality/) | Devuelve un valor que indica si esta instancia no es igual a un objeto especificado. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


