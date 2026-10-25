---
title: "WorkContourType enumı"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.WorkContourType enumı. Bir işin konturunu belirtir"
type: docs
weight: 3610
url: /tr/net/aspose.tasks/workcontourtype/
---
## WorkContourType enumeration

Bir işin konturunu belirtir.

```csharp
public enum WorkContourType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Undefined | `-1` | Değer, orijinal proje dosyasında tanımlanmamıştı. |
| Flat | `0` | Düz iş konturu. |
| BackLoaded | `1` | Arka Yüklemeli iş konturu. |
| FrontLoaded | `2` | Ön Yüklemeli iş konturu. |
| DoublePeak | `3` | Çift Zirve iş konturu. |
| EarlyPeak | `4` | Erken Zirve iş konturu. |
| LatePeak | `5` | Geç Zirve iş konturu. |
| Bell | `6` | Çan iş konturu. |
| Turtle | `7` | Kaplumbağa iş konturu. |
| Contoured | `8` | Özel iş konturu. |

## Açıklamalar

XML'e dışa aktarırken Tanımsız değerler sonuç XML'inden kaldırılacaktır.

## Örnekler

Kaynak atamaları için farklı zaman aşamalı veri konturlarının nasıl ayarlanacağını gösterir.

```csharp
var project = new Project();
project.Set(Prj.StartDate, new DateTime(2000, 1, 3, 8, 0, 0));
project.Set(Prj.FinishDate, new DateTime(2000, 1, 7, 17, 0, 0));

// bir görev ekle
var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8, TimeUnitType.Hour));
task.Set(Tsk.Finish, new DateTime(2000, 1, 3, 17, 0, 0));

var resource = project.Resources.Add("Resource");

// kaynak ataması ekle
var resourceAssignment = project.ResourceAssignments.Add(task, resource);
resourceAssignment.Set(Asn.Start, new DateTime(2000, 1, 3, 8, 0, 0));
resourceAssignment.Set(Asn.Work, project.GetWork(8));
resourceAssignment.Set(Asn.Finish, new DateTime(2000, 1, 3, 17, 0, 0));

// Düz kontur varsayılan konturdur
Console.WriteLine("Flat contour");

var collection = task.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate));
foreach (var td in collection)
{
    Console.WriteLine(td.Start.ToShortDateString() + " " + td.Value);
}

// Konturu değiştir
Console.WriteLine("Turtle contour");
resourceAssignment.Set(Asn.WorkContour, WorkContourType.Turtle);
collection = task.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate));
foreach (var td in collection)
{
    Console.WriteLine(td.Start.ToShortDateString() + " " + td.Value);
}

// Konturu değiştir
Console.WriteLine("BackLoaded contour");
resourceAssignment.Set(Asn.WorkContour, WorkContourType.BackLoaded);
collection = task.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate));
foreach (var td in collection)
{
    Console.WriteLine(td.Start.ToShortDateString() + " " + td.Value);
}

// Konturu değiştir
Console.WriteLine("FrontLoaded contour");
resourceAssignment.Set(Asn.WorkContour, WorkContourType.FrontLoaded);
collection = task.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate));
foreach (var td in collection)
{
    Console.WriteLine(td.Start.ToShortDateString() + " " + td.Value);
}

// Konturu değiştir
Console.WriteLine("Bell contour");
resourceAssignment.Set(Asn.WorkContour, WorkContourType.Bell);
collection = task.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate));
foreach (var td in collection)
{
    Console.WriteLine(td.Start.ToShortDateString() + " " + td.Value);
}

// Konturu değiştir
Console.WriteLine("EarlyPeak contour");
resourceAssignment.Set(Asn.WorkContour, WorkContourType.EarlyPeak);
collection = task.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate));
foreach (var td in collection)
{
    Console.WriteLine(td.Start.ToShortDateString() + " " + td.Value);
}

// Konturu değiştir
Console.WriteLine("LatePeak contour");
resourceAssignment.Set(Asn.WorkContour, WorkContourType.LatePeak);
collection = task.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate));
foreach (var td in collection)
{
    Console.WriteLine(td.Start.ToShortDateString() + " " + td.Value);
}

// Konturu değiştir
Console.WriteLine("DoublePeak contour");
resourceAssignment.Set(Asn.WorkContour, WorkContourType.DoublePeak);
collection = task.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate));
foreach (var td in collection)
{
    Console.WriteLine(td.Start.ToShortDateString() + " " + td.Value);
}
```

### Ayrıca Bakınız

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


