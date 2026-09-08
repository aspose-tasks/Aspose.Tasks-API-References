---
title: "Класс OleObjectCollection"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.OleObjectCollection. Представляет коллекцию, содержащую экземпляры класса OleObject"
type: docs
weight: 1130
url: /ru/net/aspose.tasks/oleobjectcollection/
---
## OleObjectCollection class

Представляет коллекцию, содержащую экземпляры класса [`OleObject`](../oleobject/).

```csharp
public sealed class OleObjectCollection : IList<OleObject>
```

## Методы

| Имя | Описание |
| --- | --- |
| [Clear](../../aspose.tasks/oleobjectcollection/clear/)() | Очищает коллекцию. Чтобы сохранить эти изменения, следует вызвать project.Save с новыми MPPSaveOptions { WriteViewData = true; } |
| [GetEnumerator](../../aspose.tasks/oleobjectcollection/getenumerator/)() | Возвращает перечислитель для этой коллекции. |
| [ToList](../../aspose.tasks/oleobjectcollection/tolist/)() | Преобразует экземпляр класса `OleObjectCollection` в список, содержащий экземпляры класса [`OleObject`](../oleobject/). |

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

* class [OleObject](../oleobject/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


