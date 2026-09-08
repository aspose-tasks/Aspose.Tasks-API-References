---
title: "Перечисление Shape"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Aspose.Tasks.Visualization.Shape enum. Форма маркера в начале или в конце стиля полосы, которая будет отрисована при сохранении данных представления в некоторых форматах SaveFileFormat"
type: docs
weight: 3360
url: /ru/net/aspose.tasks.visualization/shape/
---
## Shape enumeration

Форма маркера в начале или в конце стиля полосы, которая будет отрисована при сохранении данных представления в некоторых [`SaveFileFormat`](../../aspose.tasks.saving/savefileformat/).

```csharp
public enum Shape
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| None | `0` | Указывает форму None. |
| VerticalLine | `1` | Указывает форму вертикальной линии. |
| Pentagon | `2` | Указывает форму пятиугольника. |
| Triangle | `3` | Указывает форму треугольника. |
| LeftBracket | `4` | Указывает форму левой скобки. |
| RightBracket | `5` | Указывает форму правой скобки. |
| ArrowDown | `6` | Указывает форму стрелки вниз. |
| LeftFade | `7` | Указывает форму левого затухания. |
| RightFade | `8` | Указывает форму правого затухания. |
| Diamond | `9` | Указывает форму ромба. |
| Circle | `10` | Указывает форму круга. |

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


