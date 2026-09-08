---
title: "Класс CopyToOptions"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.CopyToOptions. Позволяет указать дополнительные параметры при копировании данных проекта"
type: docs
weight: 340
url: /ru/net/aspose.tasks/copytooptions/
---
## CopyToOptions class

Позволяет указать дополнительные параметры при копировании данных проекта.

```csharp
public class CopyToOptions
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [CopyToOptions](copytooptions/)() | Инициализирует новый экземпляр класса `CopyToOptions`. |

## Свойства

| Имя | Описание |
| --- | --- |
| [CopyViewData](../../aspose.tasks/copytooptions/copyviewdata/) { get; set; } | Получает или задаёт значение, указывающее, копировать ли данные представления при копировании данных проекта. Значение по умолчанию — true. |

## Примеры

Показывает, как использовать параметры копирования проекта.

```csharp
var project = new Project(DataDir + "CopyToProjectEmpty.xml");
File.Copy(DataDir + "CopyToProjectEmpty.mpp", OutDir + "ProjectCopying_out.mpp", true);

var mppProject = new Project(OutDir + "ProjectCopying_out.mpp");

// пропустить копирование данных представления при копировании общих данных проекта.
var copyToOptions = new CopyToOptions();
copyToOptions.CopyViewData = false;
project.CopyTo(mppProject, copyToOptions);
```

### См. также

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


