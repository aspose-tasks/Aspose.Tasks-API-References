---
title: "PrimaveraXmlReader.PrimaveraXmlReader"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Конструктор PrimaveraXmlReader. Инициализирует новый экземпляр класса PrimaveraXmlReader"
type: docs
weight: 10
url: /ru/net/aspose.tasks/primaveraxmlreader/primaveraxmlreader/
---
## PrimaveraXmlReader(string) {#constructor_1}

Инициализирует новый экземпляр класса [`PrimaveraXmlReader`](../).

```csharp
public PrimaveraXmlReader(string templatePath)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| templatePath | Строка | Путь к шаблону, где находятся проект или проекты Primavera Xml |

## Примеры

Показывает, как просмотреть информацию о коротких проектах из файла Primavera XML.

```csharp
var reader = new PrimaveraXmlReader(DataDir + "MultiprojectWithExternal.xml");
var projectInfos = reader.GetProjectInfos();
foreach (var info in projectInfos)
{
    Console.WriteLine("{0} - '{1}' - {2}", info.Uid, info.Name, info.ExportFlag);
}
```

### См. также

* class [PrimaveraXmlReader](../)
* namespace [Aspose.Tasks](../../primaveraxmlreader/)
* assembly [Aspose.Tasks](../../../)

---

## PrimaveraXmlReader(Stream) {#constructor}

Инициализирует новый экземпляр класса [`PrimaveraXmlReader`](../).

```csharp
public PrimaveraXmlReader(Stream stream)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| поток | Поток | Поток, содержащий содержимое Primavera Xml. |

## Примеры

Показывает, как импортировать проект из потока Primavera XML.

```csharp
using (var stream = new FileStream(DataDir + "primavera.xml", FileMode.Open))
{
    var reader = new PrimaveraXmlReader(stream);
    List<int> projectUids = reader.GetProjectUids();
    foreach (var projectUid in projectUids)
    {
        Console.WriteLine("Project UID: " + projectUid);
    }
}
```

### См. также

* class [PrimaveraXmlReader](../)
* namespace [Aspose.Tasks](../../primaveraxmlreader/)
* assembly [Aspose.Tasks](../../../)


