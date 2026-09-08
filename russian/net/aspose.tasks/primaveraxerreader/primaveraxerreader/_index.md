---
title: "PrimaveraXerReader.PrimaveraXerReader"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Конструктор PrimaveraXerReader. Инициализирует новый экземпляр класса PrimaveraXerReader"
type: docs
weight: 10
url: /ru/net/aspose.tasks/primaveraxerreader/primaveraxerreader/
---
## PrimaveraXerReader(string) {#constructor_1}

Инициализирует новый экземпляр класса [`PrimaveraXerReader`](../).

```csharp
public PrimaveraXerReader(string xerFilePath)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| xerFilePath | Строка | Путь к файлу .xer, где находятся проект или проекты Primavera. |

## Примеры

Показывает, как просмотреть информацию о кратких проектах из файла Primavera XER.

```csharp
var reader = new PrimaveraXerReader(DataDir + "MultiprojectWithExternal.xer");
var projectInfos = reader.GetProjectInfos();
foreach (var info in projectInfos)
{
    Console.WriteLine("{0} - '{1}' - {2}", info.Uid, info.Name, info.ExportFlag);
}

var project = reader.LoadProject(5494);

Console.WriteLine("Loaded project '{0}' with Uid {1}", project.Name, project.Uid);
```

### См. также

* class [PrimaveraXerReader](../)
* namespace [Aspose.Tasks](../../primaveraxerreader/)
* assembly [Aspose.Tasks](../../../)

---

## PrimaveraXerReader(Stream) {#constructor}

Инициализирует новый экземпляр класса [`PrimaveraXerReader`](../).

```csharp
public PrimaveraXerReader(Stream stream)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| поток | Поток | Поток с содержимым Primavera XER. |

### См. также

* class [PrimaveraXerReader](../)
* namespace [Aspose.Tasks](../../primaveraxerreader/)
* assembly [Aspose.Tasks](../../../)


