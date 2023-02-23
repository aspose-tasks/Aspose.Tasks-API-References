---
title: OleObjectCollection.Clear
second_title: Aspose.Tasks for .NET API 参考
description: OleObjectCollection 方法. 清除集合为了保留这些更改 project.Save 应该使用新的 MPPSaveOptions  WriteViewData  true 
type: docs
weight: 10
url: /zh/net/aspose.tasks/oleobjectcollection/clear/
---
## OleObjectCollection.Clear method

清除集合。为了保留这些更改 project.Save 应该使用新的 MPPSaveOptions { WriteViewData = true; }

```csharp
public void Clear()
```

### 例子

如何清除 OLE 对象并保留这些更改。

```csharp
[C#]
project.OleObjects.Clear();
project.Save("output.mpp", new MPPSaveOptions {WriteViewData = true;} )
```

### 也可以看看

* class [OleObjectCollection](../)
* 命名空间 [Aspose.Tasks](../../oleobjectcollection/)
* 部件 [Aspose.Tasks](../../../)


