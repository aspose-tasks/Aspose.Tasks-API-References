---
title: "Project.Set"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод Project. Сопоставляет указанное свойство с указанным значением в этом контейнере"
type: docs
weight: 1240
url: /ru/net/aspose.tasks/project/set/
---
## Set&lt;T&gt;(Key&lt;T, PrjKey&gt;, T) {#set_1}

Сопоставляет указанное свойство с указанным значением в этом контейнере.

```csharp
public void Set<T>(Key<T, PrjKey> key, T val)
```

| Параметр | Описание |
| --- | --- |
| T | тип сопоставленного значения. |
| key | указанный ключ свойства. [`Prj`](../../prj/) для получения ключа свойства. |
| значение | значение. |

## Примеры

Показывает, как установить атрибуты задачи.

```csharp
var project = new Project();
project.Set(Prj.NewTaskStartDate, TaskStartDateType.CurrentDate);
project.Save(OutDir + "SetAttributesForNewTasks_out.xml", SaveFileFormat.Xml);
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Set(Key&lt;DateTime, PrjKey&gt;, DateTime) {#set}

Сопоставляет указанное свойство с указанным значением в этом контейнере.

```csharp
public void Set(Key<DateTime, PrjKey> key, DateTime val)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| key | Key`2 | указанный ключ свойства. [`Prj`](../../prj/) для получения ключа свойства. |
| значение | DateTime | значение. |

## Примеры

Показывает, как установить атрибуты задачи.

```csharp
var project = new Project();
project.Set(Prj.NewTaskStartDate, TaskStartDateType.CurrentDate);
project.Save(OutDir + "SetAttributesForNewTasks_out.xml", SaveFileFormat.Xml);
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


