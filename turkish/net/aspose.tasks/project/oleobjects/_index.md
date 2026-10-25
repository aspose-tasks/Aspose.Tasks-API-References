---
title: "Project.OleObjects"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Project özelliği. Bu proje dosyasına bağlı veya gömülü olan OleObject sınıfının örneklerini içeren bir koleksiyon alır. Yalnızca mpp dosya formatı için kullanılabilir. Bu koleksiyon, Clear işlemi dışında yalnızca okunur."
type: docs
weight: 700
url: /tr/net/aspose.tasks/project/oleobjects/
---
## Project.OleObjects property

Bu proje dosyasına bağlı veya gömülü olan [`OleObject`](../../oleobject/) sınıfının örneklerini içeren bir koleksiyon alır. Yalnızca mpp dosya formatı için kullanılabilir. Bu koleksiyon, 'Clear' işlemi dışında yalnızca okunur.

```csharp
public OleObjectCollection OleObjects { get; }
```

## Örnekler

Gömülü OLE nesnelerinin nasıl çıkarılacağını gösterir.

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

### Ayrıca Bakınız

* class [OleObjectCollection](../../oleobjectcollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


