---
title: "MPPSaveOptions.ClearVba"
second_title: "Aspose.Tasks for .NET API 参考"
description: "MPPSaveOptions 属性。获取或设置一个值，指示在将项目保存为 MPP 格式时是否移除现有的 VBA 宏数据。"
type: docs
weight: 20
url: /zh/net/aspose.tasks.saving/mppsaveoptions/clearvba/
---
## MPPSaveOptions.ClearVba property

获取或设置一个值，指示在将项目保存为 MPP 格式时是否删除现有的 VBA 宏数据。

```csharp
public bool ClearVba { get; set; }
```

## 示例

展示如何从 MPP 文件中删除 VBA 宏。

```csharp
var project = new Project(DataDir + "VbaProject.mpp");
project.Save(OutDir + "Vba.cleared.mpp", new MPPSaveOptions() { ClearVba = true });
```

### 另见

* class [MPPSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../mppsaveoptions/)
* assembly [Aspose.Tasks](../../../)


