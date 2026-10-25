---
title: "Перечисление Timescale"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Aspose.Tasks.Visualization.Timescale enum. Определяет параметры, которые указывают, как отображать шкалу времени в представлениях Gantt Chart Task Usage или Resource Usage при экспорте проекта в графический формат."
type: docs
weight: 3430
url: /ru/net/aspose.tasks.visualization/timescale/
---
## Timescale enumeration

Определяет параметры, которые указывают, как отображать шкалу времени в представлениях Gantt Chart, Task Usage или Resource Usage при экспорте проекта в графический формат.

```csharp
public enum Timescale
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| DefinedInView | `0` | Используйте настройки шкалы времени, определённые в свойствах представления проекта: [`BottomTimescaleTier`](../../aspose.tasks/ganttchartview/bottomtimescaletier/), [`MiddleTimescaleTier`](../../aspose.tasks/ganttchartview/middletimescaletier/), [`TopTimescaleTier`](../../aspose.tasks/ganttchartview/toptimescaletier/). Действительно для форматов, содержащих данные представления. Например, проекты, считанные из формата MPP. |
| Days | `1` | Предопределённая двухуровневая шкала времени, где минимальный уровень детализации — один день. |
| ThirdsOfMonths | `10` | Предопределённая двухуровневая шкала времени, где уровень детализации — одна треть месяца. |
| Months | `30` | Предопределённая двухуровневая шкала времени, где минимальный уровень детализации — один месяц. |

## Примеры

Показывает, как сохранить проект в виде SVG‑файла.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");
SaveOptions options = new SvgOptions
                        {
                            // установите <see cref=\"P:Aspose.Tasks.Saving.SaveOptions.PresentationFormat\" /> в котором будет сохранён документ
                            PresentationFormat = PresentationFormat.GanttChart,

                            // установите значение, указывающее, следует ли увеличивать высоту строки, чтобы вместить её содержимое
                            FitContent = true,

                            // установите минимальный временной интервал для рендеринга. Значение по умолчанию — <see cref=\"P:Aspose.Tasks.Saving.SaveOptions.Timescale\">Days</see>
                            Timescale = Timescale.ThirdsOfMonths,

                            // определяет, следует ли использовать градиентную кисть при рендеринге макета проекта
                            // В настоящее время использование градиентной кисти не поддерживается при рендеринге в SVG.
                            // UseGradientBrush = true
                        };
project.Save(OutDir + "UseSvgOptions_out.svg", options);
```

### См. также

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


