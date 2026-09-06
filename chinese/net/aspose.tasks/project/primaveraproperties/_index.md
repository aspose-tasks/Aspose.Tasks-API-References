---
title: "Project.PrimaveraProperties"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Project 属性。获取一个对象，其中包含从 Primavera 文件读取的项目的 Primavera 特定属性。"
type: docs
weight: 720
url: /zh/net/aspose.tasks/project/primaveraproperties/
---
## Project.PrimaveraProperties property

获取一个对象，其中包含从 Primavera 文件读取的项目的 Primavera 特定属性。

```csharp
public PrimaveraProjectProperties PrimaveraProperties { get; }
```

## 示例

展示如何从 Primavera 文件读取项目并检查项目的 Primavera 特定属性。

```csharp
var options = new PrimaveraReadOptions();
options.ProjectUid = 4861;

// 返回具有特殊 UID 的项目
var project = new Project(DataDir + "ScheduleOptions.xer", options);

// 如果项目的计划选项具有默认值，则 PrimaveraProperties 可以为 null。
if (project.PrimaveraProperties != null)
{
    Console.WriteLine("Project's schedule options:");
    Console.WriteLine("Relationship Lag Calendar: " + project.PrimaveraProperties.RelationshipLagCalendar);
    Console.WriteLine("Make Open Ended Activities Critical: " + project.PrimaveraProperties.MakeOpenEndedActivitiesCritical);
    Console.WriteLine("Ignore Other Project Relationships: " + project.PrimaveraProperties.IgnoreOtherProjectRelationships);
    Console.WriteLine("Use Expected Finish Dates: " + project.PrimaveraProperties.UseExpectedFinishDates);

    Console.WriteLine("How critical activities are defined: " +
                      project.PrimaveraProperties.CriticalActivitiesDefiningMethod);

    if (project.PrimaveraProperties.CriticalActivitiesDefiningMethod == PrimaveraCriticalActivitiesDefiningMethod.TotalFloat)
    {
        Console.WriteLine("Total Float threshold for critical activities: " + project.PrimaveraProperties.CriticalTotalFloatLimit);
    }
}
```

### 另见

* class [PrimaveraProjectProperties](../../primaveraprojectproperties/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


