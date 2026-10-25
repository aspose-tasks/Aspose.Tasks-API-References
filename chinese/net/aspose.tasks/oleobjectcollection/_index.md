---
title: "类 OleObjectCollection"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.OleObjectCollection 类。表示一个包含 OleObject 类实例的集合。"
type: docs
weight: 1130
url: /zh/net/aspose.tasks/oleobjectcollection/
---
## OleObjectCollection class

表示一个包含 [`OleObject`](../oleobject/) 类实例的集合。

```csharp
public sealed class OleObjectCollection : IList<OleObject>
```

## 方法

| 名称 | 描述 |
| --- | --- |
| [Clear](../../aspose.tasks/oleobjectcollection/clear/)() | 清除集合。为了持久化这些更改，应该使用 new MPPSaveOptions { WriteViewData = true; } 调用 project.Save。 |
| [GetEnumerator](../../aspose.tasks/oleobjectcollection/getenumerator/)() | 返回此集合的枚举器。 |
| [ToList](../../aspose.tasks/oleobjectcollection/tolist/)() | 将 `OleObjectCollection` 类的实例转换为包含 [`OleObject`](../oleobject/) 类实例的列表。 |

## 示例

展示如何使用 OLE 对象集合。

```csharp
IDictionary<string, string> extensions = new Dictionary<string, string>
{
    { "RTF", "_rtfFile_out.rtf" },
    { "MSWordDoc", "_wordFile_out.docx" },
    { "ExcelML12", "_excelFile_out.xlsx" }
};

var project = new Project(DataDir + "Embedded.mpp");

// 通过使用索引访问
// List<OleObject> list = project.OleObjects.ToList();
// for (var index = 0; index < list.Count; index++)
// {
// var oleObject = list[index];
// }

// 或者枚举可以遍历 OLE 对象
foreach (var oleObject in project.OleObjects)
{
    if (string.IsNullOrEmpty(oleObject.FileFormat) || !extensions.ContainsKey(oleObject.FileFormat))
    {
        continue;
    }

    var path = OutDir + "EmbeddedContent_" + extensions[oleObject.FileFormat];
    using (var stream = new FileStream(path, FileMode.Create))
    {
        stream.Write(oleObject.Content, 0, oleObject.Content.Length);
    }
}
```

### 另见

* class [OleObject](../oleobject/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


