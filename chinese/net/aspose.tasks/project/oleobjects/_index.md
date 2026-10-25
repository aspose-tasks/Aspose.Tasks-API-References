---
title: "Project.OleObjects"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Project 属性。获取一个集合，其中包含链接或嵌入到此项目文件的 OleObject 类实例。仅适用于 mpp 文件格式。此集合为只读，除 Clear 操作外。"
type: docs
weight: 700
url: /zh/net/aspose.tasks/project/oleobjects/
---
## Project.OleObjects property

获取一个集合，其中包含链接或嵌入到此项目文件的 [`OleObject`](../../oleobject/) 类实例。仅适用于 mpp 文件格式。此集合为只读，除 'Clear' 操作外。

```csharp
public OleObjectCollection OleObjects { get; }
```

## 示例

展示如何提取嵌入的 OLE 对象。

```csharp
IDictionary<string, string> formatExt = new Dictionary<string, string>
{
    { "RTF", "_rtfFile_out.rtf" },
    { "MSWordDoc", "_wordFile_out.docx" },
    { "ExcelML12", "_excelFile_out.xlsx" }
};

var project = new Project(DataDir + "Embedded.mpp");

foreach (var oleObject in project.OleObjects)
{
    if (string.IsNullOrEmpty(oleObject.FileFormat) || !formatExt.ContainsKey(oleObject.FileFormat))
    {
        continue;
    }

    var path = OutDir + "EmbeddedContent_" + formatExt[oleObject.FileFormat];
    using (var stream = new FileStream(path, FileMode.Create))
    {
        stream.Write(oleObject.Content, 0, oleObject.Content.Length);
    }
}
```

### 另见

* class [OleObjectCollection](../../oleobjectcollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


