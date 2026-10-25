---
title: "SvgOptions.SvgOptions"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Конструктор SvgOptions. Инициализирует новый экземпляр класса SvgOptions, который может использоваться для сохранения проекта в формате SVG."
type: docs
weight: 10
url: /ru/net/aspose.tasks.saving/svgoptions/svgoptions/
---
## SvgOptions constructor

Инициализирует новый экземпляр класса [`SvgOptions`](../), который может использоваться для сохранения проекта в формате SVG.

```csharp
public SvgOptions()
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


