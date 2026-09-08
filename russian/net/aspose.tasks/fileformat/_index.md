---
title: "Перечисление FileFormat"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Перечисление Aspose.Tasks.FileFormat. Указывает формат файлов проекта"
type: docs
weight: 590
url: /ru/net/aspose.tasks/fileformat/
---
## FileFormat enumeration

Указывает формат файла проекта.

```csharp
public enum FileFormat
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Undefined | `0` | Не может быть определено. |
| P6XML | `1` | Представляет формат Primavera P6 XML. |
| XML | `2` | Формат Microsoft Project XML. |
| MPP8 | `3` | Формат Microsoft Project 2000. |
| MPP9 | `4` | Формат Microsoft Project 2003. |
| MPP12 | `5` | Формат Microsoft Project 2007. |
| MPP14 | `6` | Формат Microsoft Project 2010. |
| MPT9 | `7` | Формат шаблона Microsoft Project 2003. |
| MPT12 | `8` | Формат шаблона Microsoft Project 2007. |
| MPT14 | `9` | Формат шаблона Microsoft Project 2010 (2013). |
| MPX | `10` | Формат файла Mpx |
| XER | `11` | Представляет формат Primavera XER |
| HTML | `12` | Представляет формат HTML |
| ProjectServer | `13` | Проект был считан из Project Server или Project Online |

## Примеры

Показывает, как читать формат файла проверки проекта.

```csharp
var info = Project.GetProjectFileInfo(DataDir + "Project.xml");
Console.WriteLine("CanRead: " + info.CanRead);
Console.WriteLine("ProjectApplicationInfo: " + info.ProjectApplicationInfo);
Console.WriteLine("ProjectFileFormat: " + info.ProjectFileFormat);
```

### См. также

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


