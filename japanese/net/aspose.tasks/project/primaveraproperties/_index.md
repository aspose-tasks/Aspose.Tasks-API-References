---
title: "Project.PrimaveraProperties"
second_title: "Aspose.Tasks for .NET API リファレンス"
description: "Project プロパティ。Primavera ファイルから読み込まれたプロジェクトの Primavera 固有プロパティを含むオブジェクトを取得します。"
type: docs
weight: 720
url: /ja/net/aspose.tasks/project/primaveraproperties/
---
## Project.PrimaveraProperties property

Primavera ファイルから読み込まれたプロジェクトの Primavera 固有プロパティを含むオブジェクトを取得します。

```csharp
public PrimaveraProjectProperties PrimaveraProperties { get; }
```

## 例

Primavera ファイルからプロジェクトを読み取り、プロジェクトの Primavera 固有プロパティを調べる方法を示します。

```csharp
var options = new PrimaveraReadOptions();
options.ProjectUid = 4861;

// 特別な Uid を持つプロジェクトを返します。
var project = new Project(DataDir + "ScheduleOptions.xer", options);

// プロジェクトのスケジュールオプションがデフォルト値の場合、PrimaveraProperties は null になる可能性があります。
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

### 関連項目

* class [PrimaveraProjectProperties](../../primaveraprojectproperties/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


