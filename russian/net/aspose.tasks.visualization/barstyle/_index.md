---
title: "Класс BarStyle"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.Visualization.BarStyle. Изменяет визуальный стиль полосы для элемента в представлении проекта."
type: docs
weight: 2960
url: /ru/net/aspose.tasks.visualization/barstyle/
---
## BarStyle class

Изменить визуальный стиль полосы для элемента в представлении проекта.

```csharp
public class BarStyle
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [BarStyle](barstyle/)() | Инициализирует новый экземпляр класса `BarStyle`. |

## Свойства

| Имя | Описание |
| --- | --- |
| [BarColor](../../aspose.tasks.visualization/barstyle/barcolor/) { get; set; } | Получает или задает цвет стиля полосы. |
| [BarShape](../../aspose.tasks.visualization/barstyle/barshape/) { get; set; } | Получает или задает [`BarShape`](./barshape/) стиля полосы. |
| [BottomBarTextConverter](../../aspose.tasks.visualization/barstyle/bottombartextconverter/) { get; set; } | Получает или задает пользовательский конвертер для получения текста, отображаемого внизу полосы задачи. Переопределяет значение свойства [`BottomField`](./bottomfield/). |
| [BottomField](../../aspose.tasks.visualization/barstyle/bottomfield/) { get; set; } | Получает или задает поле, отображаемое в нижней части полосы. |
| [EndShape](../../aspose.tasks.visualization/barstyle/endshape/) { get; set; } | Получает или задает [`Shape`](../shape/) в конце полосы. |
| [EndShapeColor](../../aspose.tasks.visualization/barstyle/endshapecolor/) { get; set; } | Получает или задает цвет формы в конце полосы. |
| [EndShapeType](../../aspose.tasks.visualization/barstyle/endshapetype/) { get; set; } | Получает или задает тип формы конца. [`GanttBarType`](../ganttbartype/). |
| [From](../../aspose.tasks.visualization/barstyle/from/) { get; set; } | Получает или задает позицию начальной точки диаграммы Ганта. [`Field`](../../aspose.tasks/field/). |
| [InsideBarTextConverter](../../aspose.tasks.visualization/barstyle/insidebartextconverter/) { get; set; } | Получает или задает пользовательский конвертер для получения текста, отображаемого внутри полосы задачи. Переопределяет значение свойства [`InsideField`](./insidefield/). |
| [InsideField](../../aspose.tasks.visualization/barstyle/insidefield/) { get; set; } | Получает или задает поле, отображаемое внутри полосы. |
| [ItemType](../../aspose.tasks.visualization/barstyle/itemtype/) { get; set; } | Получает или задает [`BarItemType`](../baritemtype/) стиля полосы. |
| [LeftBarTextConverter](../../aspose.tasks.visualization/barstyle/leftbartextconverter/) { get; set; } | Получает или задает пользовательский конвертер для получения текста, отображаемого слева от полосы задачи. Переопределяет значение свойства [`LeftField`](./leftfield/). |
| [LeftField](../../aspose.tasks.visualization/barstyle/leftfield/) { get; set; } | Получает или задает поле, отображаемое слева от полосы. |
| [RightBarTextConverter](../../aspose.tasks.visualization/barstyle/rightbartextconverter/) { get; set; } | Получает или задает пользовательский конвертер для получения текста, отображаемого справа от полосы задачи. Переопределяет значение свойства [`RightField`](./rightfield/). |
| [RightField](../../aspose.tasks.visualization/barstyle/rightfield/) { get; set; } | Получает или задает поле, отображаемое справа от полосы. |
| [StartShape](../../aspose.tasks.visualization/barstyle/startshape/) { get; set; } | Получает или задает [`Shape`](../shape/) в начале полосы. |
| [StartShapeColor](../../aspose.tasks.visualization/barstyle/startshapecolor/) { get; set; } | Получает или задает цвет формы в начале полосы. |
| [StartShapeType](../../aspose.tasks.visualization/barstyle/startshapetype/) { get; set; } | Получает или задает тип формы начала. |
| [TextStyle](../../aspose.tasks.visualization/barstyle/textstyle/) { get; set; } | Получает или задает стиль текста полосы. |
| [To](../../aspose.tasks.visualization/barstyle/to/) { get; set; } | Получает или задает позицию конечной точки полосы Ганта. |
| [TopBarTextConverter](../../aspose.tasks.visualization/barstyle/topbartextconverter/) { get; set; } | Получает или задает пользовательский конвертер для получения текста, отображаемого в верхней части полосы задачи. Переопределяет значение свойства [`TopField`](./topfield/). |
| [TopField](../../aspose.tasks.visualization/barstyle/topfield/) { get; set; } | Получает или задает поле, отображаемое в верхней части полосы. |

## Примеры

Показывает, как использовать пользовательские стили полос.

```csharp
var project = new Project(DataDir + "Project2.mpp");
SaveOptions options = new PdfSaveOptions
{
    BarStyles = new List<BarStyle>()
};

// добавить стиль полосы для задач‑контрольных точек
var style = new BarStyle();
// установить <see cref="T:Aspose.Tasks.Visualization.BarItemType" /> стиля полосы
style.ItemType = BarItemType.Milestone;
// установить <see cref="T:System.Drawing.Color" /> стиля полосы.
style.BarColor = Color.Green;
// установить <see cref="P:Aspose.Tasks.Visualization.BarStyle.BarShape" /> стиля полосы
style.BarShape = BarShape.HalfHeight;
// установить <see cref=\"T:Aspose.Tasks.Visualization.Shape\" /> в начале полосы
style.StartShape = Shape.LeftBracket;
// установить <see cref=\"T:System.Drawing.Color\" /> формы в начале полосы
style.StartShapeColor = Color.Aqua;
// установить <see cref=\"T:Aspose.Tasks.Visualization.Shape\" /> в конце полосы
style.EndShape = Shape.RightBracket;
// установить <see cref=\"T:System.Drawing.Color\" /> формы в конце полосы
style.EndShapeColor = Color.Aquamarine;
// установить текст для отображения справа от полосы.
style.TextStyle = new TextStyle();
style.TextStyle.BackgroundColor = Color.Black;

// существует функция, позволяющая преобразовать текст полосы.
// установим конвертер, чтобы получить текст для отображения полосы.
style.LeftBarTextConverter = task =>
{
    if (!task.Get(Tsk.Name).StartsWith("T"))
    {
        task.Set(Tsk.Name, "T" + task.Get(Tsk.Name));
    }

    return task.Get(Tsk.Name);
};

options.BarStyles.Add(style);

// сохранить проект
project.Save(OutDir + "WorkWithBarStyle_out.mpp", options);
```

### См. также

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


