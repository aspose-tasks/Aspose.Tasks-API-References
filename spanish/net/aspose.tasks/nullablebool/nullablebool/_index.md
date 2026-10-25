---
title: "NullableBool.NullableBool"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Constructor NullableBool. Inicializa una nueva instancia de la estructura NullableBool con el valor booleano especificado."
type: docs
weight: 10
url: /es/net/aspose.tasks/nullablebool/nullablebool/
---
## NullableBool(bool) {#constructor}

Inicializa una nueva instancia de la estructura [`NullableBool`](../) con el valor booleano especificado.

```csharp
public NullableBool(bool value)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | Boolean | el valor booleano especificado. |

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

---

## NullableBool(bool, bool) {#constructor_1}

Inicializa una nueva instancia de la estructura [`NullableBool`](../).

```csharp
public NullableBool(bool value, bool isDefined)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | Boolean | El valor actual. |
| isDefined | Boolean | El valor que indica si el valor actual está definido. |

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


