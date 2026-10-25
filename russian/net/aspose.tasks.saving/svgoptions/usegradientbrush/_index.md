---
title: "SvgOptions.UseGradientBrush"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство SvgOptions. Определяет, следует ли использовать градиентную кисть при рендеринге макета проекта. В настоящее время использование градиентной кисти не поддерживается при рендеринге в SVG."
type: docs
weight: 30
url: /ru/net/aspose.tasks.saving/svgoptions/usegradientbrush/
---
## SvgOptions.UseGradientBrush property

Определяет, следует ли использовать градиентную кисть при рендеринге макета проекта. В настоящее время использование градиентной кисти не поддерживается при рендеринге в SVG.

```csharp
public override bool UseGradientBrush { get; set; }
```

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

* class [SvgOptions](../)
* namespace [Aspose.Tasks.Saving](../../svgoptions/)
* assembly [Aspose.Tasks](../../../)


