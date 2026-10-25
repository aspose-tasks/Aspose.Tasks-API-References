---
title: "Class GroupCriterion"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Aspose.Tasks.GroupCriterion class. Mewakili kriteria dalam definisi grup. Objek GroupCriterion merupakan anggota dari koleksi GroupCriterionCollection."
type: docs
weight: 790
url: /id/net/aspose.tasks/groupcriterion/
---
## GroupCriterion class

Mewakili kriteria dalam definisi grup. Objek GroupCriterion merupakan anggota dari koleksi [`GroupCriterionCollection`](../groupcriterioncollection/).

```csharp
public class GroupCriterion
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [GroupCriterion](groupcriterion/)() | Konstruktor default. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [Ascending](../../aspose.tasks/groupcriterion/ascending/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah field yang digunakan sebagai kriteria dalam definisi grup diurutkan secara naik. False jika field diurutkan secara turun. |
| [CellColor](../../aspose.tasks/groupcriterion/cellcolor/) { get; set; } | Mendapatkan atau mengatur warna latar belakang sel untuk field yang digunakan sebagai kriteria dalam definisi grup. |
| [Field](../../aspose.tasks/groupcriterion/field/) { get; set; } | Mendapatkan atau mengatur field yang dikelompokkan. |
| [Font](../../aspose.tasks/groupcriterion/font/) { get; set; } | Mendapatkan atau mengatur font untuk kriteria dalam definisi grup. |
| [FontColor](../../aspose.tasks/groupcriterion/fontcolor/) { get; set; } | Mendapatkan atau mengatur warna font untuk field yang digunakan sebagai kriteria dalam definisi grup. |
| [GroupInterval](../../aspose.tasks/groupcriterion/groupinterval/) { get; set; } | Mendapatkan atau mengatur interval untuk field yang digunakan sebagai kriteria dalam definisi grup. |
| [GroupOn](../../aspose.tasks/groupcriterion/groupon/) { get; set; } | Mendapatkan atau mengatur tipe pengelompokan untuk field yang digunakan sebagai kriteria dalam definisi grup. |
| [Pattern](../../aspose.tasks/groupcriterion/pattern/) { get; set; } | Mendapatkan atau mengatur pola sel untuk bidang yang digunakan sebagai kriteria dalam definisi grup. |
| [StartAt](../../aspose.tasks/groupcriterion/startat/) { get; set; } | Mendapatkan atau mengatur awal interval untuk bidang yang digunakan sebagai kriteria dalam definisi grup. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| override [Equals](../../aspose.tasks/groupcriterion/equals/)(object) | Kembalikan nilai yang menunjukkan apakah instance ini sama dengan objek yang ditentukan. |
| override [GetHashCode](../../aspose.tasks/groupcriterion/gethashcode/)() | Berfungsi sebagai fungsi hash untuk tipe tertentu. |

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

Menampilkan cara menambahkan grup ke proyek.

```csharp
var p = new Project();

{
    var group = new Group();
    group.Name = "My new task group";
    group.MaintainHierarchy = true;
    group.ShowSummary = true;

    var criterion = new GroupCriterion();
    criterion.Field = Field.TaskDuration1;
    criterion.Font = new FontDescriptor("Comic Sans MS", 13F, FontStyles.Italic);
    criterion.GroupOn = GroupOn.DurationMinutes;
    criterion.StartAt = 5;
    criterion.GroupInterval = 3D;
    criterion.Pattern = BackgroundPattern.DarkDiagonalLeft;
    group.GroupCriteria.Add(criterion);

    var criterion2 = new GroupCriterion();
    criterion2.Field = Field.TaskPercentComplete;
    criterion2.Font = new FontDescriptor("Bodoni MT", 17, FontStyles.Italic | FontStyles.Bold);
    criterion2.GroupOn = GroupOn.Pct199;
    criterion2.Pattern = BackgroundPattern.LightDither;
    criterion2.CellColor = Color.Green;
    criterion2.FontColor = Color.Red;
    group.GroupCriteria.Add(criterion2);
    group.GroupAssignments = true;
    p.TaskGroups.Add(group);
}

{
    var group = new Group();
    group.Name = "My new resource group";
    group.MaintainHierarchy = true;
    group.ShowSummary = true;

    var criterion = new GroupCriterion();
    criterion.Field = Field.ResourceDuration1;
    criterion.Font = new FontDescriptor("Comic Sans MS", 11F, FontStyles.Bold);
    criterion.GroupOn = GroupOn.DurationHours;
    criterion.StartAt = 1;
    criterion.GroupInterval = 2D;
    criterion.Pattern = BackgroundPattern.DarkDiagonalLeft;
    group.GroupCriteria.Add(criterion);

    var criterion2 = new GroupCriterion();
    criterion2.Field = Field.ResourceCost;
    criterion2.Font = new FontDescriptor("Bodoni MT", 12, FontStyles.Italic | FontStyles.Bold);
    criterion2.GroupOn = GroupOn.Interval;
    criterion2.StartAt = 1D;
    criterion2.GroupInterval = 10D;
    criterion2.Pattern = BackgroundPattern.LightDither;
    criterion2.CellColor = Color.Magenta;
    criterion2.FontColor = Color.Red;
    group.GroupCriteria.Add(criterion2);
    group.GroupAssignments = true;
    p.ResourceGroups.Add(group);
}

p.Save(OutDir + "output_CreateGroup.mpp", new MPPSaveOptions() { WriteGroups = true });
```

### Lihat Juga

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


