---
title: "AssignmentBaseline.CompareTo"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "AssignmentBaseline metode. Implementasi antarmuka IComparable. Membandingkan instance ini dengan objek Baseline yang ditentukan"
type: docs
weight: 50
url: /id/net/aspose.tasks/assignmentbaseline/compareto/
---
## AssignmentBaseline.CompareTo method

Implementasi antarmuka IComparable. Membandingkan instance ini dengan objek Baseline yang ditentukan.

```csharp
public int CompareTo(AssignmentBaseline other)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| lain | AssignmentBaseline | objek Baseline yang ditentukan untuk dibandingkan dengan instance ini. |

### Nilai Kembali

mengembalikan -1 jika instance ini lebih kecil dari objek yang ditentukan, 1 jika instance ini lebih besar dari objek yang ditentukan; jika tidak, mengembalikan 0

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

* class [AssignmentBaseline](../)
* namespace [Aspose.Tasks](../../assignmentbaseline/)
* assembly [Aspose.Tasks](../../../)


