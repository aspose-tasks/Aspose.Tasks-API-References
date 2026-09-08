---
title: "Класс OleObject"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.OleObject. Представляет объект OLE, который может быть вставлен в представление диаграммы Ганта файла MPP."
type: docs
weight: 1120
url: /ru/net/aspose.tasks/oleobject/
---
## OleObject class

Представляет объект OLE, который может быть вставлен в представление Gantt Chart View MPP‑файла.

```csharp
public class OleObject
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [OleObject](oleobject/)() | Инициализирует новый экземпляр класса `OleObject`. |

## Свойства

| Имя | Описание |
| --- | --- |
| [ApplicationName](../../aspose.tasks/oleobject/applicationname/) { get; set; } | Получает или задает имя приложения, с помощью которого открывается встроенный объект. |
| [Content](../../aspose.tasks/oleobject/content/) { get; set; } | Получает или задает данные встроенного файла; null, если данные не были встроены. |
| [DisplayAsIcon](../../aspose.tasks/oleobject/displayasicon/) { get; set; } | Получает или задает флаг, указывающий, должно ли объект OLE отображаться в виде значка или в виде обычного изображения. |
| [FileFormat](../../aspose.tasks/oleobject/fileformat/) { get; set; } | Получает или задает формат файла встроенного объекта. |
| [FullPath](../../aspose.tasks/oleobject/fullpath/) { get; set; } | Получает или задает полный путь вставленного объекта. |
| [Id](../../aspose.tasks/oleobject/id/) { get; set; } | Получает или задает идентификатор объекта. |
| [Label](../../aspose.tasks/oleobject/label/) { get; set; } | Получает или задает метку вставленного объекта. |
| [Linked](../../aspose.tasks/oleobject/linked/) { get; } | Получает значение, указывающее, содержит ли файл проекта только ссылку на фактические данные, хранящиеся в источнике ссылки. |
| [Name](../../aspose.tasks/oleobject/name/) { get; set; } | Получает или задает имя экземпляра объекта OLE. |
| [TemporaryFile](../../aspose.tasks/oleobject/temporaryfile/) { get; set; } | Получает или задает путь к временному файлу вставленного объекта. |
| [View](../../aspose.tasks/oleobject/view/) { get; set; } | Получает или задает экземпляр класса [`View`](./view/), к которому относится вставленный объект. |

## Примеры

Показано, как читать информацию об объектах OLE.

```csharp
[Test]
public void WorkWithOleObject()
{
    var images = new Project(DataDir + "TaskImage2010.mpp");
    List<OleObject> oleObjects = images.OleObjects.ToList();

    Console.WriteLine("Ole Objects Count: " + oleObjects.Count);
    foreach (var oleObject in oleObjects)
    {
        Console.WriteLine(" Id: " + oleObject.Id);
        Console.WriteLine(" Name: " + oleObject.Name);
        Console.WriteLine(" DisplayAsIcon: " + oleObject.DisplayAsIcon);
        Console.WriteLine(" Application Name: " + oleObject.ApplicationName);
        Console.WriteLine(" File Format: " + oleObject.FileFormat);
        Console.WriteLine(" Label: " + oleObject.Label);
        Console.WriteLine(" Full Path: " + oleObject.FullPath);
        Console.WriteLine(" Is Linked: " + oleObject.Linked);
        Console.WriteLine(" View Name: " + oleObject.View.Name);
        Console.WriteLine(" Content (first 10 bytes): " + this.Get10Bytes(oleObject));
    }
}

private string Get10Bytes(OleObject oleObject)
{
    byte[] bytes = oleObject.Content;
    var chunk = new byte[10];
    Array.Copy(bytes, chunk, 10);
    var builder = new StringBuilder();
    foreach (var b in chunk)
    {
        builder.Append(b + ", ");
    }

    builder.Remove(builder.Length - 3, 1);
    return builder.ToString();
}
```

### См. также

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


