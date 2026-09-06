---
title: "类 Baseline"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.Baseline 类。表示资源的基线值"
type: docs
weight: 110
url: /zh/net/aspose.tasks/baseline/
---
## Baseline class

表示资源的基线值。

```csharp
public class Baseline : IComparable<Baseline>, IEquatable<Baseline>
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [Baseline](baseline/)() | 默认构造函数。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [BaselineNumber](../../aspose.tasks/baseline/baselinenumber/) { get; set; } | 获取或设置基线数据记录的唯一编号。 |
| [Bcwp](../../aspose.tasks/baseline/bcwp/) { get; set; } | 获取或设置资源在项目截至目前执行的工作的预算成本。 |
| [Bcws](../../aspose.tasks/baseline/bcws/) { get; set; } | 获取或设置为资源计划的工作的预算成本。 |
| [Cost](../../aspose.tasks/baseline/cost/) { get; set; } | 获取或设置基线保存时资源的预计成本。 |
| [Work](../../aspose.tasks/baseline/work/) { get; set; } | 获取或设置基线保存时分配给资源的工作量。基线保存时分配给资源的工作量。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| [CompareTo](../../aspose.tasks/baseline/compareto/)(Baseline) | IComparable 接口实现。将此实例与指定的 Baseline 对象进行比较。 |
| [Equals](../../aspose.tasks/baseline/equals/#equals)(Baseline) | 返回一个值，指示此实例是否等于指定的对象。 |
| override [Equals](../../aspose.tasks/baseline/equals/#equals_1)(object) | 返回一个值，指示此实例是否等于指定的对象。 |
| override [GetHashCode](../../aspose.tasks/baseline/gethashcode/)() | 返回基线的哈希码值。 |
| [operator ==](../../aspose.tasks/baseline/op_equality/) | 返回一个值，指示此实例是否等于指定的对象。 |
| [operator &gt;](../../aspose.tasks/baseline/op_greaterthan/) | 返回一个值，指示此实例是否大于指定的对象。 |
| [operator &gt;=](../../aspose.tasks/baseline/op_greaterthanorequal/) | 返回一个值，指示此实例是否大于或等于指定的对象。 |
| [operator !=](../../aspose.tasks/baseline/op_inequality/) | 返回一个值，指示此实例是否不等于指定的对象。 |
| [operator &lt;](../../aspose.tasks/baseline/op_lessthan/) | 返回一个值，指示此实例是否小于指定的对象。 |
| [operator &lt;=](../../aspose.tasks/baseline/op_lessthanorequal/) | 返回一个值，指示此实例是否小于或等于指定的对象。 |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


