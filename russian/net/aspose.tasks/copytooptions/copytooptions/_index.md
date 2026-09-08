---
title: "CopyToOptions.CopyToOptions"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Конструктор CopyToOptions. Инициализирует новый экземпляр класса CopyToOptions"
type: docs
weight: 10
url: /ru/net/aspose.tasks/copytooptions/copytooptions/
---
## CopyToOptions constructor

Инициализирует новый экземпляр класса [`CopyToOptions`](../).

```csharp
public CopyToOptions()
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


