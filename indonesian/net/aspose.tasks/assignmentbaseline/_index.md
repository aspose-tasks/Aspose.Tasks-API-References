---
title: "Kelas AssignmentBaseline"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.AssignmentBaseline. Mewakili Baseline dari penugasan sumber daya"
type: docs
weight: 50
url: /id/net/aspose.tasks/assignmentbaseline/
---
## AssignmentBaseline class

Mewakili Baseline dari penugasan sumber daya.

```csharp
public class AssignmentBaseline : Baseline, IComparable<AssignmentBaseline>, 
    IEquatable<AssignmentBaseline>
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [AssignmentBaseline](assignmentbaseline/)() | Konstruktor default. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [BaselineNumber](../../aspose.tasks/baseline/baselinenumber/) { get; set; } | Mendapatkan atau mengatur nomor unik dari catatan data baseline. |
| [Bcwp](../../aspose.tasks/baseline/bcwp/) { get; set; } | Mendapatkan atau mengatur biaya yang dianggarkan untuk pekerjaan yang dilakukan oleh sumber daya untuk proyek hingga saat ini. |
| [Bcws](../../aspose.tasks/baseline/bcws/) { get; set; } | Mendapatkan atau mengatur biaya anggaran dari pekerjaan yang dijadwalkan untuk sebuah sumber daya. |
| [Cost](../../aspose.tasks/baseline/cost/) { get; set; } | Mendapatkan atau mengatur biaya proyeksi sumber daya ketika baseline disimpan. |
| [Finish](../../aspose.tasks/assignmentbaseline/finish/) { get; set; } | Mendapatkan atau mengatur tanggal selesai terjadwal dari penugasan sumber daya ketika baseline disimpan. Tanggal selesai penugasan sumber daya ketika baseline ini disimpan. |
| [Start](../../aspose.tasks/assignmentbaseline/start/) { get; set; } | Mendapatkan atau mengatur tanggal mulai terjadwal dari penugasan sumber daya ketika baseline disimpan. Tanggal mulai penugasan sumber daya ketika baseline ini disimpan. |
| [TimephasedData](../../aspose.tasks/assignmentbaseline/timephaseddata/) { get; set; } | Mendapatkan atau mengatur instance [`TimephasedDataCollection`](../timephaseddatacollection/) untuk objek ini. Data berwaktu yang terkait dengan baseline penugasan sumber daya. Mengembalikan instance [`TimephasedDataCollection`](../timephaseddatacollection/) untuk objek ini. Kumpulan data berwaktu yang terkait dengan baseline ini. |
| [Work](../../aspose.tasks/baseline/work/) { get; set; } | Mendapatkan atau mengatur pekerjaan yang ditugaskan ke sumber daya ketika baseline disimpan. Jumlah pekerjaan yang ditugaskan ke sumber daya ketika baseline disimpan. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| [CompareTo](../../aspose.tasks/assignmentbaseline/compareto/#compareto)(AssignmentBaseline) | Implementasi antarmuka IComparable. Membandingkan instance ini dengan objek Baseline yang ditentukan. |
| [CompareTo](../../aspose.tasks/baseline/compareto/)(Baseline) | Implementasi antarmuka IComparable. Membandingkan instance ini dengan objek Baseline yang ditentukan. |
| [Equals](../../aspose.tasks/assignmentbaseline/equals/#equals)(AssignmentBaseline) | Kembalikan nilai yang menunjukkan apakah instance ini sama dengan objek AssignmentBaseline yang ditentukan. |
| [Equals](../../aspose.tasks/baseline/equals/)(Baseline) | Kembalikan nilai yang menunjukkan apakah instance ini sama dengan objek yang ditentukan. |
| override [Equals](../../aspose.tasks/assignmentbaseline/equals/#equals_2)(object) | Kembalikan nilai yang menunjukkan apakah instance ini sama dengan objek yang ditentukan. |
| override [GetHashCode](../../aspose.tasks/assignmentbaseline/gethashcode/)() |  |

## Contoh

Menampilkan cara bekerja dengan baseline penugasan.

```csharp
var project = new Project(DataDir + "AssignmentBaseline2007.mpp");

// baseline penugasan diatur ketika seseorang mengatur baseline pada seluruh proyek
project.SetBaseline(BaselineType.Baseline);

// baca informasi baseline penugasan
foreach (var assignment in project.ResourceAssignments)
{
    foreach (var baseline in assignment.Baselines)
    {
        Console.WriteLine("Baseline Start: " + baseline.Start);
        Console.WriteLine("Baseline Finish: " + baseline.Finish);
        Console.WriteLine("Baseline Number: " + baseline.BaselineNumber);
        Console.WriteLine("Bcwp: " + baseline.Bcwp);
        Console.WriteLine("Bcws: " + baseline.Bcws);
        Console.WriteLine("Cost: " + baseline.Cost);
        Console.WriteLine("Work: " + baseline.Work);
        if (baseline.TimephasedData != null)
        {
            foreach (var td in baseline.TimephasedData)
            {
                Console.WriteLine("TD Start: " + td.Start);
                Console.WriteLine("TD Finish: " + td.Finish);
                Console.WriteLine("TD Timephased Data Type: " + td.TimephasedDataType);
                Console.WriteLine();
            }
        }

        Console.WriteLine();
    }

    Console.WriteLine();
}

// periksa kesetaraan baseline
var assn1 = project.ResourceAssignments.GetByUid(5);
var assn2 = project.ResourceAssignments.GetByUid(7);

var assignmentBaseline1 = assn1.Baselines.ToList()[0];
var assignmentBaseline2 = assn2.Baselines.ToList()[0];

// baseline dapat dibandingkan dengan menggunakan overload metode 'Equals'
Console.WriteLine("Are baselines equal: " + assignmentBaseline1.Equals(assignmentBaseline2));

// atau dengan menggunakan operasi aritmetika yang di‑overload
Console.WriteLine("Is baseline 1 less than baseline 2: " + (assignmentBaseline1 < assignmentBaseline2));

// hashcode baseline didasarkan pada nomor baseline
Console.WriteLine("Assignment baseline 1 hashcode: " + assignmentBaseline1.GetHashCode());
Console.WriteLine("Assignment baseline 2 hashcode: " + assignmentBaseline2.GetHashCode());
```

### Lihat Juga

* class [Baseline](../baseline/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


