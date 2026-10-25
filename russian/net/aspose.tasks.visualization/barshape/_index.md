---
title: "Перечисление BarShape"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Перечисление Aspose.Tasks.Visualization.BarShape. Форма прямоугольника полосы"
type: docs
weight: 2950
url: /ru/net/aspose.tasks.visualization/barshape/
---
## BarShape enumeration

Форма прямоугольника полосы.

```csharp
public enum BarShape
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Full | `0` | Указывает форму полной прямоугольной полосы. |
| HalfHeight | `1` | Указывает форму прямоугольной полосы половинной высоты, выровненной по верхнему краю. |
| HalfHeightBottom | `2` | Указывает форму прямоугольной полосы половинной высоты, выровненной по нижнему краю. |
| Thin | `3` | Указывает форму линии, выровненной по центру. |
| None | `4` | Указывает отсутствие формы полосы. |
| Middle | `5` | Указывает форму линии, выровненной по центру. |
| LineBottom | `6` | Указывает форму линии, выровненной по нижнему краю. |
| LineTop | `7` | Указывает форму линии, выровненной по верхнему краю. |

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


