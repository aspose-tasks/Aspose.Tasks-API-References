---
title: "Prj.MinutesPerWeek"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Prj alanı. Haftalık dakika sayısı"
type: docs
weight: 480
url: /tr/net/aspose.tasks/prj/minutesperweek/
---
## Prj.MinutesPerWeek field

Hafta başına dakika sayısı.

```csharp
public static readonly Key<int, PrjKey> MinutesPerWeek;
```

## Örnekler

Projenin hafta içi özelliklerinin nasıl okunup yazılacağını gösterir.

```csharp
var project = new Project(DataDir + "WriteWeekdayProperties.mpp");

// Hafta içi özelliklerini ayarla
project.Set(Prj.WeekStartDay, DayType.Monday);
project.Set(Prj.DaysPerMonth, 24);
project.Set(Prj.MinutesPerDay, 540);
project.Set(Prj.MinutesPerWeek, 3240);

// Hafta içi özelliklerini göster
Console.WriteLine("Week Start Date: " + project.Get(Prj.WeekStartDay));
Console.WriteLine("Days Per Month: " + project.Get(Prj.DaysPerMonth));
Console.WriteLine("Minutes Per Day: " + project.Get(Prj.MinutesPerDay));
Console.WriteLine("Minutes Per Week: " + project.Get(Prj.MinutesPerWeek));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


