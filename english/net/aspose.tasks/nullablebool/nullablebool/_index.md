---
title: NullableBool.NullableBool
second_title: Aspose.Tasks for .NET API Reference
description: NullableBool constructor. Initializes a new instance of the NullableBool struct with the specified boolean value
type: docs
weight: 10
url: /net/aspose.tasks/nullablebool/nullablebool/
---
## NullableBool(bool) {#constructor}

Initializes a new instance of the [`NullableBool`](../) struct with the specified boolean value.

```csharp
public NullableBool(bool value)
```

| Parameter | Type | Description |
| --- | --- | --- |
| value | Boolean | the specified boolean value. |

## Examples

Shows how to work with &lt;see cref="NullableBool" /&gt; class.

```csharp
var project = new Project();

// lets check where the <see cref="Aspose.Tasks.NullableBool" /> class is used
// the main advantage of <see cref="Aspose.Tasks.NullableBool" /> that 
// one can set it as undefined through constructing
var actualsInSync = new NullableBool(false, false);
Console.WriteLine("'ActualsInSync' Value: " + actualsInSync.Value);
Console.WriteLine("'ActualsInSync' Is Defined: " + actualsInSync.IsDefined);

// ...
// use nullable bool instance
project.Set(Prj.ActualsInSync, actualsInSync);

// ...
var honorConstraints = new NullableBool(true);
Console.WriteLine("'HonorConstraints' ToString: " + honorConstraints.ToString());

// ...
// use nullable bool instance
project.Set(Prj.HonorConstraints, honorConstraints);

// ...
```

### See Also

* struct [NullableBool](../)
* namespace [Aspose.Tasks](../../nullablebool/)
* assembly [Aspose.Tasks](../../../)

---

## NullableBool(bool, bool) {#constructor_1}

Initializes a new instance of the [`NullableBool`](../) struct.

```csharp
public NullableBool(bool value, bool isDefined)
```

| Parameter | Type | Description |
| --- | --- | --- |
| value | Boolean | The current value. |
| isDefined | Boolean | The value indicating whether current value is defined. |

## Examples

Shows how to work with &lt;see cref="NullableBool" /&gt; class.

```csharp
var project = new Project();

// lets check where the <see cref="Aspose.Tasks.NullableBool" /> class is used
// the main advantage of <see cref="Aspose.Tasks.NullableBool" /> that 
// one can set it as undefined through constructing
var actualsInSync = new NullableBool(false, false);
Console.WriteLine("'ActualsInSync' Value: " + actualsInSync.Value);
Console.WriteLine("'ActualsInSync' Is Defined: " + actualsInSync.IsDefined);

// ...
// use nullable bool instance
project.Set(Prj.ActualsInSync, actualsInSync);

// ...
var honorConstraints = new NullableBool(true);
Console.WriteLine("'HonorConstraints' ToString: " + honorConstraints.ToString());

// ...
// use nullable bool instance
project.Set(Prj.HonorConstraints, honorConstraints);

// ...
```

### See Also

* struct [NullableBool](../)
* namespace [Aspose.Tasks](../../nullablebool/)
* assembly [Aspose.Tasks](../../../)


