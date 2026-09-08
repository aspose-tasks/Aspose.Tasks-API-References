---
title: "Project.CopyTo"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод Project. Копирует основные данные и свойства проекта в другой проект."
type: docs
weight: 1060
url: /ru/net/aspose.tasks/project/copyto/
---
## CopyTo(Project) {#copyto}

Копирует основные данные и свойства проекта в другой проект.

```csharp
public void CopyTo(Project another)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| другой | Project | Другой проект, в который копировать данные. |

## Примеры

Показывает, как скопировать данные проекта в другой проект.

```csharp
var project = new Project(DataDir + "CopyToProjectEmpty.xml");
File.Copy(DataDir + "CopyToProjectEmpty.mpp", DataDir + "ProjectCopying_out.mpp", true);

var mppProject = new Project(DataDir + "ProjectCopying_out.mpp");

// пропустить копирование данных представления при копировании общих данных проекта.
project.CopyTo(mppProject);
```

### См. также

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## CopyTo(Project, CopyToOptions) {#copyto_1}

Копирует основные данные и свойства проекта в другой проект.

```csharp
public void CopyTo(Project another, CopyToOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| другой | Project | Другой проект, в который копировать данные. |
| опции | CopyToOptions | Параметры копирования для управления процессом копирования. |

## Примеры

Показывает, как скопировать проект с использованием экземпляра &lt;see cref="Aspose.Tasks.CopyToOptions"/&gt;.

```csharp
var project = new Project(DataDir + "CopyToProjectEmpty.xml");
File.Copy(DataDir + "CopyToProjectEmpty.mpp", OutDir + "ProjectCopying_out.mpp", true);

var mppProject = new Project(OutDir + "ProjectCopying_out.mpp");

// пропустить копирование данных представления при копировании общих данных проекта.
var options = new CopyToOptions
{
    CopyViewData = false
};
project.CopyTo(mppProject, options);
```

### См. также

* class [CopyToOptions](../../copytooptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


