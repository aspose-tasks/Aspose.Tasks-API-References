---
title: "类 AssignmentBaseline"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.AssignmentBaseline 类。表示资源分配的基线"
type: docs
weight: 50
url: /zh/net/aspose.tasks/assignmentbaseline/
---
## AssignmentBaseline class

表示资源分配的基线。

```csharp
public class AssignmentBaseline : Baseline, IComparable<AssignmentBaseline>, 
    IEquatable<AssignmentBaseline>
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [AssignmentBaseline](assignmentbaseline/)() | 默认构造函数。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [BaselineNumber](../../aspose.tasks/baseline/baselinenumber/) { get; set; } | 获取或设置基线数据记录的唯一编号。 |
| [Bcwp](../../aspose.tasks/baseline/bcwp/) { get; set; } | 获取或设置资源在项目截至目前执行的工作的预算成本。 |
| [Bcws](../../aspose.tasks/baseline/bcws/) { get; set; } | 获取或设置为资源计划的工作的预算成本。 |
| [Cost](../../aspose.tasks/baseline/cost/) { get; set; } | 获取或设置基线保存时资源的预计成本。 |
| [Finish](../../aspose.tasks/assignmentbaseline/finish/) { get; set; } | 获取或设置基线保存时资源分配的计划完成日期。此基线保存时资源分配的完成日期。 |
| [Start](../../aspose.tasks/assignmentbaseline/start/) { get; set; } | 获取或设置基线保存时资源分配的计划开始日期。此基线保存时资源分配的开始日期。 |
| [TimephasedData](../../aspose.tasks/assignmentbaseline/timephaseddata/) { get; set; } | 获取或设置此对象的[`TimephasedDataCollection`](../timephaseddatacollection/)实例。与资源分配基线关联的时间分段数据。返回此对象的[`TimephasedDataCollection`](../timephaseddatacollection/)实例。此基线关联的时间分段数据集合。 |
| [Work](../../aspose.tasks/baseline/work/) { get; set; } | 获取或设置基线保存时分配给资源的工作量。基线保存时分配给资源的工作量。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| [CompareTo](../../aspose.tasks/assignmentbaseline/compareto/#compareto)(AssignmentBaseline) | IComparable 接口实现。将此实例与指定的 Baseline 对象进行比较。 |
| [CompareTo](../../aspose.tasks/baseline/compareto/)(Baseline) | IComparable 接口实现。将此实例与指定的 Baseline 对象进行比较。 |
| [Equals](../../aspose.tasks/assignmentbaseline/equals/#equals)(AssignmentBaseline) | 返回一个值，指示此实例是否等于指定的 AssignmentBaseline 对象。 |
| [Equals](../../aspose.tasks/baseline/equals/)(Baseline) | 返回一个值，指示此实例是否等于指定的对象。 |
| override [Equals](../../aspose.tasks/assignmentbaseline/equals/#equals_2)(object) | 返回一个值，指示此实例是否等于指定的对象。 |
| override [GetHashCode](../../aspose.tasks/assignmentbaseline/gethashcode/)() |  |

## 示例

展示如何处理分配的基线。

```csharp
var project = new Project(DataDir + "AssignmentBaseline2007.mpp");

// 当在整个项目上设置基线时，分配基线会被设置。
project.SetBaseline(BaselineType.Baseline);

// 读取分配基线信息。
foreach (var assignment in project.ResourceAssignments)
{
    foreach (var baseline in assignment.Baselines)
    {
        Console.WriteLine("Baseline Start: " + baseline.Start);
        Console.WriteLine("Baseline Finish: " + baseline.Finish);
        Console.WriteLine("Baseline Number: " + baseline.BaselineNumber);
        Console.WriteLine("Bcwp: " + baseline.Bcwp);
        Console.WriteLine("Bcws: " + baseline.Bcws);
        Console.WriteLine("Cost: " + baseline.Cost);
        Console.WriteLine("Work: " + baseline.Work);
        if (baseline.TimephasedData != null)
        {
            foreach (var td in baseline.TimephasedData)
            {
                Console.WriteLine("TD Start: " + td.Start);
                Console.WriteLine("TD Finish: " + td.Finish);
                Console.WriteLine("TD Timephased Data Type: " + td.TimephasedDataType);
                Console.WriteLine();
            }
        }

        Console.WriteLine();
    }

    Console.WriteLine();
}

// 检查基线相等性。
var assn1 = project.ResourceAssignments.GetByUid(5);
var assn2 = project.ResourceAssignments.GetByUid(7);

var assignmentBaseline1 = assn1.Baselines.ToList()[0];
var assignmentBaseline2 = assn2.Baselines.ToList()[0];

// 可以通过使用 'Equals' 方法重载来比较基线。
Console.WriteLine("Are baselines equal: " + assignmentBaseline1.Equals(assignmentBaseline2));

// 或通过使用重载的算术运算。
Console.WriteLine("Is baseline 1 less than baseline 2: " + (assignmentBaseline1 < assignmentBaseline2));

// 基线的哈希码基于基线编号。
Console.WriteLine("Assignment baseline 1 hashcode: " + assignmentBaseline1.GetHashCode());
Console.WriteLine("Assignment baseline 2 hashcode: " + assignmentBaseline2.GetHashCode());
```

### 另见

* class [Baseline](../baseline/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


