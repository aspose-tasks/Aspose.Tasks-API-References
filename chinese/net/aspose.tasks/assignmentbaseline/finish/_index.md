---
title: "AssignmentBaseline.Finish"
second_title: "Aspose.Tasks for .NET API 参考"
description: "AssignmentBaseline 属性。获取或设置基线保存时资源分配的计划完成日期。此基线保存时资源分配的完成日期。"
type: docs
weight: 20
url: /zh/net/aspose.tasks/assignmentbaseline/finish/
---
## AssignmentBaseline.Finish property

获取或设置基线保存时资源分配的计划完成日期。此基线保存时资源分配的完成日期。

```csharp
public DateTime? Finish { get; set; }
```

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

* class [AssignmentBaseline](../)
* namespace [Aspose.Tasks](../../assignmentbaseline/)
* assembly [Aspose.Tasks](../../../)


