---
title: "OleObjectCollection.ToList"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод OleObjectCollection. Преобразует экземпляр класса OleObjectCollection в список, содержащий экземпляры класса OleObject."
type: docs
weight: 30
url: /ru/net/aspose.tasks/oleobjectcollection/tolist/
---
## OleObjectCollection.ToList method

Преобразует экземпляр класса [`OleObjectCollection`](../) в список, содержащий экземпляры класса [`OleObject`](../../oleobject/).

```csharp
public List<OleObject> ToList()
```

### Возвращаемое значение

Преобразованный в список экземпляр класса [`OleObjectCollection`](../), содержащий экземпляры класса [`OleObject`](../../oleobject/).

## Примеры

Показывает, как работать с коллекцией OLE‑объектов.

```csharp
IDictionary<string, string> extensions = new Dictionary<string, string>
{
    { "RTF", "_rtfFile_out.rtf" },
    { "MSWordDoc", "_wordFile_out.docx" },
    { "ExcelML12", "_excelFile_out.xlsx" }
};

var project = new Project(DataDir + "Embedded.mpp");

// с использованием доступа по индексу
// List<OleObject> list = project.OleObjects.ToList();
// for (var index = 0; index < list.Count; index++)
// {
// var oleObject = list[index];
// }

// или перечисление, можно перебрать OLE‑объекты
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

### См. также

* class [OleObject](../../oleobject/)
* class [OleObjectCollection](../)
* namespace [Aspose.Tasks](../../oleobjectcollection/)
* assembly [Aspose.Tasks](../../../)


