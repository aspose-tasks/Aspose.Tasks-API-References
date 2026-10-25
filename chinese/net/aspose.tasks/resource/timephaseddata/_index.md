---
title: "Resource.TimephasedData"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Resource 属性。获取或设置此对象的 TimephasedDataCollection 类实例"
type: docs
weight: 740
url: /zh/net/aspose.tasks/resource/timephaseddata/
---
## Resource.TimephasedData property

获取或设置此对象的 [`TimephasedDataCollection`](../../timephaseddatacollection/) 类的实例。

```csharp
public TimephasedDataCollection TimephasedData { get; set; }
```

## 备注

仅支持 XML 格式的读取。

## 示例

展示如何读取资源的时间分段数据。

```csharp
resource.Set(Rsc.Work, resource.ParentProject.GetWork(2));

project.SetBaseline(BaselineType.Baseline);

// 遍历资源的时间分段数据
foreach (var td in resource.TimephasedData)
{
    Console.WriteLine(td.Start);
    Console.WriteLine(td.Finish);
}
```

### 另见

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


