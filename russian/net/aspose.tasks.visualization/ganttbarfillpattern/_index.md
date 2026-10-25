---
title: "Перечисление GanttBarFillPattern"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Перечисление Aspose.Tasks.Visualization.GanttBarFillPattern. Шаблон заливки формы."
type: docs
weight: 3040
url: /ru/net/aspose.tasks.visualization/ganttbarfillpattern/
---
## GanttBarFillPattern enumeration

Шаблон заливки формы.

```csharp
public enum GanttBarFillPattern
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Hollow | `0` | Пустой шаблон. |
| SolidFill | `1` | Сплошной шаблон заполнения. |
| LightFill | `2` | Светлый шаблон заполнения. |
| MediumFill | `3` | Средний шаблон заполнения. |
| DarkFill | `4` | Темный шаблон заполнения. |
| DiagonalLeft | `5` | Диагональный левый шаблон (от верхнего левого к нижнему правому). |
| DiagonalRight | `6` | Диагональный правый шаблон (от верхнего правого к нижнему левому). |
| DiagonalCross | `7` | Диагональный крестовой шаблон. |
| LineVertical | `8` | Шаблон вертикальной линии. |
| LineHorizontal | `9` | Шаблон горизонтальной линии. |
| LineCross | `10` | Шаблон пересечения линий. |
| SolidFillWithDashedBorder | `11` | Шаблон сплошного с пунктирной границей. |

## Примеры

Показывает, как задать пользовательские стили полос в представлении проекта диаграммы Ганта.

```csharp
public void ImplementCustomBarStyle()
{
    try
    {
        var project = new Project(DataDir + "Blank2010.mpp");
        project.RootTask.Children.Add("Task");

        var view = (GanttChartView)project.DefaultView;
        var custom = GetCustomBarStyle();

        // Добавьте пользовательский стиль полосы в коллекцию пользовательских полос представления проекта
        view.CustomBarStyles.Add(custom);

        SimpleSaveOptions options = new MPPSaveOptions
        {
            WriteViewData = true
        };

        project.Save(OutDir + "ImplementCustomBarStyleWriting_out.mpp", options);
    }
    catch (NotSupportedException ex)
    {
        Console.WriteLine(
            ex.Message
            + "\nThis example will only work if you apply a valid Aspose License. You can purchase full license or get 30 day temporary license from http://www.aspose.com/purchase/default.aspx.");
    }
}

public static GanttBarStyle GetCustomBarStyle()
{
    var style = new GanttBarStyle
    {
        ShowForTaskUid = 1,
        MiddleShape = GanttBarMiddleShape.RectangleBottom,
        MiddleFillPattern = GanttBarFillPattern.MediumFill,
        MiddleShapeColor = Color.Blue,

        StartShape = GanttBarEndShape.ArrowDown,
        StartShapeColor = Color.Red,

        EndShape = GanttBarEndShape.ArrowUp,
        EndShapeColor = Color.Yellow,

        LeftField = Field.TaskResourceNames,
        RightField = Field.TaskName,
        TopField = Field.TaskStart,
        BottomField = Field.TaskFinish,
        InsideField = Field.TaskDuration
    };

    return style;
}
```

### См. также

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


