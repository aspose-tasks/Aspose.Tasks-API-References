---
title: Enum ResourceType
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.ResourceType enum. Specifies the type of a resource
type: docs
weight: 1770
url: /net/aspose.tasks/resourcetype/
---
## ResourceType enumeration

Specifies the type of a resource.

```csharp
public enum ResourceType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Material | `0` | Indicates Material resource type. |
| Work | `1` | Indicates Work resource type. |
| Cost | `2` | Indicates Cost resource type. |

## Examples

Shows how to work with resource types.

```csharp
var project = new Project();

// add a work resource
var work = project.Resources.Add("Work resource");
work.Set(Rsc.Type, ResourceType.Work);

// add a material resource
var material = project.Resources.Add("Material resource");
material.Set(Rsc.Type, ResourceType.Material);
material.Set(Rsc.MaterialLabel, "kg");

// add a material resource
var cost = project.Resources.Add("Cost resource");
cost.Set(Rsc.Type, ResourceType.Cost);
cost.Set(Rsc.Cost, 59.99m);

// work with resources: create tasks, assign resources and so on...
```

### See Also

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


