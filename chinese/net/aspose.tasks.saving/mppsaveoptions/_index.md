---
title: "类 MPPSaveOptions"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.Saving.MPPSaveOptions 类。允许在将项目数据保存为 MPP 时指定其他选项"
type: docs
weight: 2050
url: /zh/net/aspose.tasks.saving/mppsaveoptions/
---
## MPPSaveOptions class

允许在将项目数据保存为 MPP 时指定附加选项。

```csharp
public class MPPSaveOptions : SimpleSaveOptions
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [MPPSaveOptions](mppsaveoptions/)() | 初始化 `MPPSaveOptions` 类的新实例。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [ClearVba](../../aspose.tasks.saving/mppsaveoptions/clearvba/) { get; set; } | 获取或设置一个值，指示在将项目保存为 MPP 格式时是否删除现有的 VBA 宏数据。 |
| [ProtectionPassword](../../aspose.tasks.saving/mppsaveoptions/protectionpassword/) { get; set; } | 获取或设置用于保护生成的 MPP 文件的密码。当前支持 MS Project 2010 及更高版本的格式。空值表示项目文件未受保护。 |
| [RemoveInvalidAssignments](../../aspose.tasks.saving/mppsaveoptions/removeinvalidassignments/) { get; set; } | 获取或设置一个值，指示在保存为 MPP 时是否删除无效的资源分配。MS Project 会为每个任务创建一个空的资源分配。将此标志设为 true 可在保存时删除它们。 |
| [SaveFormat](../../aspose.tasks.saving/simplesaveoptions/saveformat/) { get; } | 获取或设置如果使用此保存选项对象，文档将被保存的格式。 |
| [TasksComparer](../../aspose.tasks.saving/simplesaveoptions/taskscomparer/) { get; set; } | 获取或设置用于在甘特图和任务表图上排序任务的比较器。 |
| [TasksFilter](../../aspose.tasks.saving/simplesaveoptions/tasksfilter/) { get; set; } | 获取或设置用于过滤在甘特图、任务表和任务使用图上渲染的任务的条件。 |
| [WriteFilters](../../aspose.tasks.saving/mppsaveoptions/writefilters/) { get; set; } | 获取或设置一个值，指示在将项目保存为 MPP 格式时是否写入过滤器数据。过滤器数据包括 Project.TaskFilters 和 Project.ResourceFilters 集合。 |
| [WriteGroups](../../aspose.tasks.saving/mppsaveoptions/writegroups/) { get; set; } | 获取或设置一个值，指示在将项目保存为 MPP 格式时是否写入分组数据。分组数据包括 Project.TaskGroups 和 Project.ResourceGroups 集合。 |
| [WriteVba](../../aspose.tasks.saving/mppsaveoptions/writevba/) { get; set; } | 获取或设置一个值，指示是否在 MPP 文件中更新现有的 VBA 宏数据。当前支持写入 VbaModule.SourceCode。 |
| [WriteViewData](../../aspose.tasks.saving/mppsaveoptions/writeviewdata/) { get; set; } | 获取或设置一个值，指示在将项目保存为 MPP 格式时是否写入视图数据。视图数据包括 Project.Views、Filters 和 Tables 集合。 |

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

* class [SimpleSaveOptions](../simplesaveoptions/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


