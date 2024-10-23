---
title: Struct NullableBool
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.NullableBool struct. A class for boolean values with possibility to check whether the value was defined or not
type: docs
weight: 1090
url: /net/aspose.tasks/nullablebool/
---
## NullableBool structure

A class for boolean values with possibility to check whether the value was defined or not.

```csharp
public struct NullableBool : IEquatable<NullableBool>
```

## Constructors

| Name | Description |
| --- | --- |
| [NullableBool](nullablebool/#constructor)(bool) | Initializes a new instance of the `NullableBool` struct with the specified boolean value. |
| [NullableBool](nullablebool/#constructor_1)(bool, bool) | Initializes a new instance of the `NullableBool` struct. |

## Properties

| Name | Description |
| --- | --- |
| [IsDefined](../../aspose.tasks/nullablebool/isdefined/) { get; } | Gets a value indicating whether the value was defined; otherwise, false. |
| [Value](../../aspose.tasks/nullablebool/value/) { get; set; } | Gets or sets a value indicating whether current value is true or false. |

## Methods

| Name | Description |
| --- | --- |
| [Equals](../../aspose.tasks/nullablebool/equals/#equals)(NullableBool) | Returns a flag indicating whether this instance is equal to the specified instance of the `NullableBool` class. |
| override [Equals](../../aspose.tasks/nullablebool/equals/#equals_1)(object) | Returns a flag indicating whether this instance is equal to the specified object. |
| override [GetHashCode](../../aspose.tasks/nullablebool/gethashcode/)() | Returns a hash code value for the instance of the `NullableBool` class. |
| override [ToString](../../aspose.tasks/nullablebool/tostring/)() | Returns a string that represents the current object. |
| [operator ==](../../aspose.tasks/nullablebool/op_equality/) | Returns a value indicating whether this instance is equal to a specified object. |
| [implicit operator](../../aspose.tasks/nullablebool/op_implicit/#op_implicit_1) | Implicitly converts a `NullableBool` instance to a boolean value. Returns true when [`Value`](./value/) is true and [`IsDefined`](./isdefined/) is true. (2 operators) |
| [operator !=](../../aspose.tasks/nullablebool/op_inequality/) | Returns a value indicating whether this instance is not equal to a specified object. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


