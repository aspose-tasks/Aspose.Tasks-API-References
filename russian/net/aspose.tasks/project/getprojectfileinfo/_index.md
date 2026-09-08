---
title: "Project.GetProjectFileInfo"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод Project. Читает информацию о файле проекта из файла"
type: docs
weight: 1280
url: /ru/net/aspose.tasks/project/getprojectfileinfo/
---
## GetProjectFileInfo(string) {#getprojectfileinfo_1}

Читает информацию о файле проекта из файла.

```csharp
public static ProjectFileInfo GetProjectFileInfo(string filename)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| имя файла | Строка | Имя файла проекта. |

### Возвращаемое значение

Информация о файле проекта [`ProjectFileInfo`](../../projectfileinfo/).

## Примеры

Показывает, как читать информацию о файле проекта, полученную из XML-файла.

```csharp
var info = Project.GetProjectFileInfo(DataDir + "Project.xml");
Console.WriteLine("CanRead: " + info.CanRead);
Console.WriteLine("ProjectApplicationInfo: " + info.ProjectApplicationInfo);
Console.WriteLine("ProjectFileFormat: " + info.ProjectFileFormat);
```

### См. также

* class [ProjectFileInfo](../../projectfileinfo/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetProjectFileInfo(Stream) {#getprojectfileinfo}

Получает информацию о файле проекта из потока.

```csharp
public static ProjectFileInfo GetProjectFileInfo(Stream stream)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| поток | Поток | Поток данных. |

### Возвращаемое значение

Информация о файле проекта [`ProjectFileInfo`](../../projectfileinfo/).

## Примеры

Показывает, как прочитать информацию о файле проекта XML, считанном из потока.

```csharp
using (var stream = new FileStream(DataDir + "Project.xml", FileMode.Open))
{
    var info = Project.GetProjectFileInfo(stream);
    Console.WriteLine("CanRead: " + info.CanRead);
    Console.WriteLine("ProjectApplicationInfo: " + info.ProjectApplicationInfo);
    Console.WriteLine("ProjectFileFormat: " + info.ProjectFileFormat);
}
```

### См. также

* class [ProjectFileInfo](../../projectfileinfo/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


