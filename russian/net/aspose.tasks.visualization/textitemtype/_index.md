---
title: "Перечисление TextItemType"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Aspose.Tasks.Visualization.TextItemType перечисление. Тип элемента для изменения стиля текста"
type: docs
weight: 3410
url: /ru/net/aspose.tasks.visualization/textitemtype/
---
## TextItemType enumeration

Тип элемента, для которого изменяется стиль текста.

```csharp
public enum TextItemType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| RowColumnTitles | `0` | Заголовки строк и столбцов. |
| CriticalTasks | `1` | Критические задачи. |
| NoncriticalTasks | `2` | Некритические задачи. |
| MilestoneTasks | `3` | Контрольные задачи. |
| InactiveTasks | `4` | Неактивные задачи. |
| SummaryTasks | `5` | Сводные задачи. |
| AssignmentRow | `6` | Строка назначения. |
| TopTimescaleTier | `7` | Верхний уровень шкалы времени. |
| BottomTimescaleTier | `8` | Нижний уровень шкалы времени. |
| MiddleTimescaleTier | `9` | Средний уровень шкалы времени. |
| Resources | `10` | Лист ресурсов. |
| OverallocatedResources | `11` | Перераспределённые ресурсы. |
| TaskFilterHighlight | `12` | Элемент текста выделения фильтра задачи. |
| BarTextBottom | `13` | Элемент текста нижней части полосы. |
| BarTextInside | `14` | Элемент текста внутри полосы. |
| BarTextLeft | `15` | Элемент текста слева от полосы. |
| BarTextRight | `16` | Элемент текста справа от полосы. |
| BarTextTop | `17` | Элемент текста верхней части полосы. |
| MarkedTasks | `18` | Элемент текста отмеченной задачи. |
| ProjectSummary | `19` | Элемент текста сводной задачи проекта. |
| ExternalTasks | `20` | Элемент текста внешних задач. |
| Allocated | `21` | Элемент текста распределения. |
| ChangedCells | `22` | Изменённые ячейки. |

## Примеры

Показывает, как работать с типами элементов текста.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
SaveOptions options = new PdfSaveOptions
{
    PresentationFormat = PresentationFormat.ResourceSheet
};

var style = new TextStyle(FontStyles.Italic | FontStyles.Bold)
{
    Color = Color.OrangeRed
};

style.ItemType = TextItemType.OverallocatedResources;

options.TextStyles = new List<TextStyle>
{
    style
};
project.Save(OutDir + "CustomizeTextStyle_out.pdf", options);
```

### См. также

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


