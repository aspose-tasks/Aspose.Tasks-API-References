---
title: Enum WorkGroupType
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.WorkGroupType enum. Specifies the type of a workgroup
type: docs
weight: 3590
url: /net/aspose.tasks/workgrouptype/
---
## WorkGroupType enumeration

Specifies the type of a workgroup.

```csharp
public enum WorkGroupType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Default | `0` | Indicates Default work group type. |
| None | `1` | Indicates None work group type. |
| Email | `2` | Indicates Email work group type. |
| Web | `3` | Indicates Web work group type. |

## Examples

Shows how to set work group of a resource.

```csharp
var project = new Project();

// ...
var resource = project.Resources.Add("Resource");
resource.Set(Rsc.Workgroup, WorkGroupType.Web);

// ...
```

### See Also

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


