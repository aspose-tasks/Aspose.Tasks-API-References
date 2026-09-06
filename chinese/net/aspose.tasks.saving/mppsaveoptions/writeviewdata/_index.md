---
title: "MPPSaveOptions.WriteViewData"
second_title: "Aspose.Tasks for .NET API 参考"
description: "MPPSaveOptions 属性。获取或设置一个值，指示在将项目保存为 MPP 格式时是否写入视图数据。视图数据包括 Project.Views Filters 和 Tables 集合。"
type: docs
weight: 80
url: /zh/net/aspose.tasks.saving/mppsaveoptions/writeviewdata/
---
## MPPSaveOptions.WriteViewData property

获取或设置一个值，指示在将项目保存为 MPP 格式时是否写入视图数据。视图数据包括 Project.Views、Filters 和 Tables 集合。

```csharp
public bool WriteViewData { get; set; }
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


