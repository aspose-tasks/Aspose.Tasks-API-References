---
title: "Project.OleObjects"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство Project. Получает коллекцию, содержащую экземпляры класса OleObject, которые связаны или встроены в этот файл проекта. Доступно только для формата файла mpp. Эта коллекция доступна только для чтения, за исключением операции Clear."
type: docs
weight: 700
url: /ru/net/aspose.tasks/project/oleobjects/
---
## Project.OleObjects property

Получает коллекцию, содержащую экземпляры класса [`OleObject`](../../oleobject/), которые связаны или встроены в этот файл проекта. Доступно только для формата файла mpp. Эта коллекция доступна только для чтения, за исключением операции 'Clear'.

```csharp
public OleObjectCollection OleObjects { get; }
```

## Примеры

Показывает, как извлечь встроенные OLE‑объекты.

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

### См. также

* class [OleObjectCollection](../../oleobjectcollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


