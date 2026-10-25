---
title: "OleObjectCollection.Clear"
second_title: "Aspose.Tasks for .NET API 参考"
description: "OleObjectCollection 方法。清除集合。为了持久化这些更改，应使用 new MPPSaveOptions  WriteViewData  true 调用 project.Save。"
type: docs
weight: 10
url: /zh/net/aspose.tasks/oleobjectcollection/clear/
---
## OleObjectCollection.Clear method

清除集合。为了持久化这些更改，应该使用 new MPPSaveOptions { WriteViewData = true; } 调用 project.Save。

```csharp
public void Clear()
```

## 示例

如何清除 OLE 对象并持久化这些更改。

```csharp
[C#]
project.OleObjects.Clear();
project.Save("output.mpp", new MPPSaveOptions {WriteViewData = true;} )
```

展示如何从指定项目中移除 OLE 对象。

```csharp
[Test]
public void ClearOleObjects()
{
    var project = new Project(DataDir + "TaskImage2010.mpp");
    project.OleObjects.Clear();
    project.Save(OutDir + "ClearedProject.mpp");
}
```

### 另见

* class [OleObjectCollection](../)
* namespace [Aspose.Tasks](../../oleobjectcollection/)
* assembly [Aspose.Tasks](../../../)


