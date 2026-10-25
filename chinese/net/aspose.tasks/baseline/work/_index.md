---
title: "Baseline.Work"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Baseline 属性。获取或设置基线保存时分配给资源的工作量。即基线保存时分配给资源的工作量。"
type: docs
weight: 60
url: /zh/net/aspose.tasks/baseline/work/
---
## Baseline.Work property

获取或设置基线保存时分配给资源的工作量。基线保存时分配给资源的工作量。

```csharp
public Duration Work { get; set; }
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

* struct [Duration](../../duration/)
* class [Baseline](../)
* namespace [Aspose.Tasks](../../baseline/)
* assembly [Aspose.Tasks](../../../)


