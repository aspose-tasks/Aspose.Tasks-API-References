---
title: NullableBool.IsDefined
second_title: Aspose.Tasks for .NET API Reference
description: NullableBool property. Gets a value indicating whether the value was defined otherwise false
type: docs
weight: 20
url: /net/aspose.tasks/nullablebool/isdefined/
---
## NullableBool.IsDefined property

Gets a value indicating whether the value was defined; otherwise, false.

```csharp
public bool IsDefined { get; }
```

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


