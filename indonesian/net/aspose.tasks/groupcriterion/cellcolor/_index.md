---
title: "GroupCriterion.CellColor"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "GroupCriterion properti. Mendapatkan atau mengatur warna latar belakang sel untuk bidang yang digunakan sebagai kriteria dalam definisi grup"
type: docs
weight: 30
url: /id/net/aspose.tasks/groupcriterion/cellcolor/
---
## GroupCriterion.CellColor property

Mendapatkan atau mengatur warna latar belakang sel untuk field yang digunakan sebagai kriteria dalam definisi grup.

```csharp
public Color CellColor { get; set; }
```

## Contoh

Menampilkan cara membaca properti kriteria grup.

```csharp
var project = new Project(DataDir + "ReadGroupDefinitionData.mpp");

Console.WriteLine("Task Groups Count: " + project.TaskGroups.Count);
var group = project.TaskGroups.ToList()[1];
Console.WriteLine("Task Group Name: " + group.Name);
Console.WriteLine("Task Group Criteria count: " + group.GroupCriteria.Count);

Console.WriteLine("\n************* Retrieving Task Group's Criterion information *************");
var criterion = group.GroupCriteria.ToList()[0];
Console.WriteLine("Task Criterion Field: " + criterion.Field);
Console.WriteLine("Task Criterion GroupOn: " + criterion.GroupOn);
Console.WriteLine("Task Criterion Cell Color: " + criterion.CellColor);
Console.WriteLine("Task Criterion Font Color: " + criterion.FontColor);
Console.WriteLine("Task Criterion Group Interval: " + criterion.GroupInterval);
Console.WriteLine("Task Criterion Start At: " + criterion.StartAt);

// baca pola latar belakang kriteria
Console.WriteLine("Task Criterion Pattern: " + criterion.Pattern);

Console.WriteLine("\n*********** Retrieving Criterion's Font Information ***********");
Console.WriteLine("Font Name: " + criterion.Font.FontFamily);
Console.WriteLine("Font Size: " + criterion.Font.Size);
Console.WriteLine("Font Style: " + criterion.Font.Style);
Console.WriteLine("Ascending/Descending: " + criterion.Ascending);
```

### Lihat Juga

* class [GroupCriterion](../)
* namespace [Aspose.Tasks](../../groupcriterion/)
* assembly [Aspose.Tasks](../../../)


