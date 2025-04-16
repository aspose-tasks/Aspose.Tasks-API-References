---
title: Enum TaskStartDateType
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.TaskStartDateType enum. Specifies the type of a tasks start date
type: docs
weight: 2370
url: /net/aspose.tasks/taskstartdatetype/
---
## TaskStartDateType enumeration

Specifies the type of a task's start date.

```csharp
public enum TaskStartDateType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Undefined | `-1` | The field's value was not defined in original project file. |
| ProjectStartDate | `0` | Project start date |
| CurrentDate | `1` | Current date |

## Remarks

While exporting into XML the Undefined values will be eliminated from resulting XML.

## Examples

Shows how to set task's default start date as 'CurrentDate'.

```csharp
var project = new Project();
project.Set(Prj.NewTaskStartDate, TaskStartDateType.CurrentDate);
project.Save(OutDir + "SetAttributesForNewTasks_out.xml", SaveFileFormat.Xml);
```

### See Also

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


