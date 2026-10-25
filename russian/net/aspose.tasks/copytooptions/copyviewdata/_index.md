---
title: "CopyToOptions.CopyViewData"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство CopyToOptions. Получает или задает значение, указывающее, следует ли копировать данные представления при копировании данных проекта. Значение по умолчанию — true"
type: docs
weight: 20
url: /ru/net/aspose.tasks/copytooptions/copyviewdata/
---
## CopyToOptions.CopyViewData property

Получает или задаёт значение, указывающее, копировать ли данные представления при копировании данных проекта. Значение по умолчанию — true.

```csharp
public bool CopyViewData { get; set; }
```

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

* class [CopyToOptions](../)
* namespace [Aspose.Tasks](../../copytooptions/)
* assembly [Aspose.Tasks](../../../)


