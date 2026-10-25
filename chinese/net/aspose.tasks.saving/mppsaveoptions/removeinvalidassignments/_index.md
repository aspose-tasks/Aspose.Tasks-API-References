---
title: "MPPSaveOptions.RemoveInvalidAssignments"
second_title: "Aspose.Tasks for .NET API 参考"
description: "MPPSaveOptions 属性。获取或设置一个值，指示在保存为 MPP 时是否移除无效的资源分配。MS Project 为每个任务创建一个空的资源分配。将此标志设为 true 可在保存时将其移除。"
type: docs
weight: 40
url: /zh/net/aspose.tasks.saving/mppsaveoptions/removeinvalidassignments/
---
## MPPSaveOptions.RemoveInvalidAssignments property

获取或设置一个值，指示在保存为 MPP 时是否删除无效的资源分配。MS Project 会为每个任务创建一个空的资源分配。将此标志设为 true 可在保存时删除它们。

```csharp
public bool RemoveInvalidAssignments { get; set; }
```

## 示例

展示如何将项目保存到流中为 MPP 文件。

```csharp
using (var stream = new FileStream(OutDir + "EmptyProjectSaveStream_out.xml", FileMode.Create, FileAccess.Write))
{
    var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

    // 创建保存选项
    SimpleSaveOptions options = new MPPSaveOptions
    {
        // 设置一个值，指示在保存为 MPP 时是否删除无效的资源分配
        RemoveInvalidAssignments = true
    };

    // 使用选项保存 MPP
    project.Save(stream, options);
}
```

### 另见

* class [MPPSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../mppsaveoptions/)
* assembly [Aspose.Tasks](../../../)


