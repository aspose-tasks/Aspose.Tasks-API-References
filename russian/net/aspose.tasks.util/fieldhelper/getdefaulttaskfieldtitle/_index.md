---
title: "FieldHelper.GetDefaultTaskFieldTitle"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод FieldHelper. Возвращает заголовок по умолчанию для конкретного поля задачи"
type: docs
weight: 20
url: /ru/net/aspose.tasks.util/fieldhelper/getdefaulttaskfieldtitle/
---
## FieldHelper.GetDefaultTaskFieldTitle method

Возвращает заголовок по умолчанию для конкретного поля задачи.

```csharp
public static string GetDefaultTaskFieldTitle(TaskKey taskKey)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| taskKey | TaskKey | Поле задачи для получения заголовка по умолчанию. |

### Возвращаемое значение

Заголовок по умолчанию конкретного поля задачи, если поле может отображаться в представлении MS Project, иначе null.

## Примеры

Показывает, как получить заголовок поля по умолчанию для конкретного поля задачи.

```csharp
Console.WriteLine("Title for Tsk.ActualCost: " + FieldHelper.GetDefaultTaskFieldTitle(Tsk.ActualCost.KeyType));
Console.WriteLine("Title for Tsk.PercentWorkComplete: " + FieldHelper.GetDefaultTaskFieldTitle(Tsk.PercentWorkComplete.KeyType));
```

### См. также

* enum [TaskKey](../../../aspose.tasks/taskkey/)
* class [FieldHelper](../)
* namespace [Aspose.Tasks.Util](../../fieldhelper/)
* assembly [Aspose.Tasks](../../../)


