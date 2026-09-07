---
title: "Kelas Group"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.Group. Mewakili definisi grup. Objek Group merupakan anggota koleksi ResourceGroups atau koleksi TaskGroups"
type: docs
weight: 770
url: /id/net/aspose.tasks/group/
---
## Group class

Mewakili definisi grup. Objek Group merupakan anggota koleksi ResourceGroups atau koleksi TaskGroups.

```csharp
public class Group
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [Group](group/)() | Menginisialisasi instance baru dari kelas `Group`. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [GroupAssignments](../../aspose.tasks/group/groupassignments/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah penugasan harus dikelompokkan alih-alih tugas. |
| [GroupCriteria](../../aspose.tasks/group/groupcriteria/) { get; set; } | Mendapatkan atau mengatur koleksi GroupCriteria yang mewakili bidang dalam definisi grup. |
| [MaintainHierarchy](../../aspose.tasks/group/maintainhierarchy/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah menampilkan semua tingkatan tugas ringkasan untuk subtugas dalam grup. |
| [Name](../../aspose.tasks/group/name/) { get; set; } | Mendapatkan atau mengatur nama objek Group. |
| [ShowInMenu](../../aspose.tasks/group/showinmenu/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah Project menampilkan nama grup dalam daftar drop-down Group di Ribbon. |
| [ShowSummary](../../aspose.tasks/group/showsummary/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah baris ringkasan ditampilkan untuk grup. |
| [Uid](../../aspose.tasks/group/uid/) { get; } | Mendapatkan pengidentifikasi unik dari sebuah grup. |

## Contoh

Menampilkan cara bekerja dengan grup.

```csharp
var project = new Project(DataDir + "ReadGroupDefinitionData.mpp");

Console.WriteLine("Task Groups Count: " + project.TaskGroups.Count);
var group = project.TaskGroups.ToList()[1];
Console.WriteLine("Task Group Uid: " + group.Uid);
Console.WriteLine("Task Group Name: " + group.Name);
Console.WriteLine("Is Task Group Maintain Hierarchy?: " + group.MaintainHierarchy);
Console.WriteLine("Is Task Group Show In Menu?: " + group.ShowInMenu);
Console.WriteLine("Is Task Group Show Summary?: " + group.ShowSummary);
Console.WriteLine("Is Task Group should groups Assignments instead of Tasks?: " + group.GroupAssignments);
Console.WriteLine("Task Group Criteria count: " + group.GroupCriteria.Count);
Console.WriteLine("\n************* Retrieving Task Group's Criterion information *************");

foreach (var criterion in group.GroupCriteria)
{
    Console.WriteLine("Task Criterion Field: " + criterion.Field);
    Console.WriteLine("Task Criterion GroupOn: " + criterion.GroupOn);
    Console.WriteLine("Task Criterion Cell Color: " + criterion.CellColor);
    Console.WriteLine("Task Criterion Pattern: " + criterion.Pattern);

    Console.WriteLine("Font Name: " + criterion.Font.FontFamily);
    Console.WriteLine("Font Size: " + criterion.Font.Size);
    Console.WriteLine("Font Style: " + criterion.Font.Style);
    Console.WriteLine("Ascending/Descending: " + criterion.Ascending);
}
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


