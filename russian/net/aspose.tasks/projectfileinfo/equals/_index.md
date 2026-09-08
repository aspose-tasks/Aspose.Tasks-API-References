---
title: "ProjectFileInfo.Equals"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "ProjectFileInfo метод. Возвращает значение, указывающее, равен ли этот экземпляр указанному объекту"
type: docs
weight: 50
url: /ru/net/aspose.tasks/projectfileinfo/equals/
---
## Equals(ProjectFileInfo) {#equals}

Возвращает значение, указывающее, равен ли этот экземпляр указанному объекту.

```csharp
public bool Equals(ProjectFileInfo other)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| другой | ProjectFileInfo | Указанный объект для сравнения с этим экземпляром. |

### Возвращаемое значение

Возвращает true, если указанный ProjectFileInfo и этот экземпляр имеют одинаковый формат файла и информацию о приложении.

## Примеры

Показывает, как читать информацию о файле проекта.

```csharp
var info = Project.GetProjectFileInfo(DataDir + "Project.xml");
Console.WriteLine("CanRead: " + info.CanRead);
Console.WriteLine("ProjectApplicationInfo: " + info.ProjectApplicationInfo);
Console.WriteLine("ProjectFileFormat: " + info.ProjectFileFormat);
```

### См. также

* class [ProjectFileInfo](../)
* namespace [Aspose.Tasks](../../projectfileinfo/)
* assembly [Aspose.Tasks](../../../)

---

## Equals(object) {#equals_1}

Возвращает значение, указывающее, равен ли этот экземпляр указанному объекту.

```csharp
public override bool Equals(object obj)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| obj | Объект | Указанный объект для сравнения с этим экземпляром. |

### Возвращаемое значение

Возвращает true, если указанный ProjectFileInfo и этот экземпляр имеют одинаковый формат файла и информацию о приложении.

## Примеры

Показывает, как читать информацию о файле проекта.

```csharp
var info = Project.GetProjectFileInfo(DataDir + "Project.xml");
Console.WriteLine("CanRead: " + info.CanRead);
Console.WriteLine("ProjectApplicationInfo: " + info.ProjectApplicationInfo);
Console.WriteLine("ProjectFileFormat: " + info.ProjectFileFormat);
```

### См. также

* class [ProjectFileInfo](../)
* namespace [Aspose.Tasks](../../projectfileinfo/)
* assembly [Aspose.Tasks](../../../)


