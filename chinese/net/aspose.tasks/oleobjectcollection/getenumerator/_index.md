---
title: "OleObjectCollection.GetEnumerator"
second_title: "Aspose.Tasks for .NET API 参考"
description: "OleObjectCollection 方法。返回此集合的枚举器"
type: docs
weight: 20
url: /zh/net/aspose.tasks/oleobjectcollection/getenumerator/
---
## OleObjectCollection.GetEnumerator method

返回此集合的枚举器。

```csharp
public IEnumerator<OleObject> GetEnumerator()
```

### 返回值

此集合的枚举器。

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

* class [OleObject](../../oleobject/)
* class [OleObjectCollection](../)
* namespace [Aspose.Tasks](../../oleobjectcollection/)
* assembly [Aspose.Tasks](../../../)


