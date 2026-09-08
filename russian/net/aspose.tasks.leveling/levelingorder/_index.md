---
title: "Перечисление LevelingOrder"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Перечисление Aspose.Tasks.Leveling.LevelingOrder. Определяет возможные значения порядка уравнивания"
type: docs
weight: 950
url: /ru/net/aspose.tasks.leveling/levelingorder/
---
## LevelingOrder enumeration

Определяет возможные значения порядка уравнивания.

```csharp
public enum LevelingOrder
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Standard | `1` | Учитываются следующие свойства: отношения предшественников, общий резерв (задача с большим общим резервом откладывается первой), дата начала, приоритет. Это значение по умолчанию. |
| IdOnly | `2` | Задачи откладываются в порядке возрастания Id. |
| PriorityThenStandard | `3` | Сначала учитывается приоритет, затем те же свойства, что и в Standard. |

### См. также

* namespace [Aspose.Tasks.Leveling](../../aspose.tasks.leveling/)
* assembly [Aspose.Tasks](../../)


