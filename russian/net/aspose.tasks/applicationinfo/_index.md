---
title: "Перечисление ApplicationInfo"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Перечисление Aspose.Tasks.ApplicationInfo. Указывает версию проекта, в которой был создан файл."
type: docs
weight: 10
url: /ru/net/aspose.tasks/applicationinfo/
---
## ApplicationInfo enumeration

Указывает версию проекта, в которой был создан файл.

```csharp
public enum ApplicationInfo
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Undefined | `0` | Не может быть определено. |
| MSP2000 | `1` | Файл был создан в Microsoft Project 2000/2002. |
| MSP2003 | `2` | Файл был создан в Microsoft Project 2003. |
| MSP2007 | `3` | Файл был создан в Microsoft Project 2007. |
| MSP2010 | `4` | Файл был создан в Microsoft Project 2010. |
| MSP2013 | `5` | Файл был создан в Microsoft Project 2013. |
| MSP2016 | `6` | Файл был создан в Microsoft Project 2016. |

## Примеры

Показано, как проверить информацию о приложении проекта.

```csharp
var info = Project.GetProjectFileInfo(DataDir + "Project.xml");
Console.WriteLine("CanRead: " + info.CanRead);
Console.WriteLine("ProjectApplicationInfo: " + info.ProjectApplicationInfo);
Console.WriteLine("ProjectFileFormat: " + info.ProjectFileFormat);
```

### См. также

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


