---
title: "枚举 BookingType"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.BookingType 枚举。指定资源的预订类型"
type: docs
weight: 150
url: /zh/net/aspose.tasks/bookingtype/
---
## BookingType enumeration

指定资源的预订类型。

```csharp
public enum BookingType
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| Undefined | `-1` | 指示该值未在原始项目文件中定义。 |
| Committed | `0` | 指示已提交的预订类型。 |
| Proposed | `1` | 指示拟议的预订类型。 |

## 备注

在导出为 XML 时，未定义的值将从生成的 XML 中删除。

## 示例

展示如何读取/写入 Asn.BookingType 属性。

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");
resource.Set(Rsc.Type, ResourceType.Work);

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.BookingType, BookingType.Proposed);

Console.WriteLine("Booking Type: " + assignment.Get(Asn.BookingType));
```

### 另见

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


