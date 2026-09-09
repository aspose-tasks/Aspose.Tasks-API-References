---
title: "Baseline.Bcws"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Baseline özelliği. Bir kaynak için planlanan bir işin bütçe maliyetini alır veya ayarlar"
type: docs
weight: 40
url: /tr/net/aspose.tasks/baseline/bcws/
---
## Baseline.Bcws property

Bir kaynak için planlanan işin bütçe maliyetini alır veya ayarlar.

```csharp
public double Bcws { get; set; }
```

## Örnekler

Atamaların temelleriyle nasıl çalışılacağını gösterir.

```csharp
var project = new Project(DataDir + "AssignmentBaseline2007.mpp");

// Atama temelleri, bütün proje için temel ayarlandığında belirlenir.
project.SetBaseline(BaselineType.Baseline);

// Atama temel bilgilerini oku
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

// Temel eşitliğini kontrol et
var assn1 = project.ResourceAssignments.GetByUid(5);
var assn2 = project.ResourceAssignments.GetByUid(7);

var assignmentBaseline1 = assn1.Baselines.ToList()[0];
var assignmentBaseline2 = assn2.Baselines.ToList()[0];

// Temeller, 'Equals' metodunun aşırı yüklemeleri kullanılarak karşılaştırılabilir
Console.WriteLine("Are baselines equal: " + assignmentBaseline1.Equals(assignmentBaseline2));

// veya aşırı yüklenmiş aritmetik işlem kullanılarak
Console.WriteLine("Is baseline 1 less than baseline 2: " + (assignmentBaseline1 < assignmentBaseline2));

// Temelin hash kodu, temel numarasına dayanır.
Console.WriteLine("Assignment baseline 1 hashcode: " + assignmentBaseline1.GetHashCode());
Console.WriteLine("Assignment baseline 2 hashcode: " + assignmentBaseline2.GetHashCode());
```

### Ayrıca Bakınız

* class [Baseline](../)
* namespace [Aspose.Tasks](../../baseline/)
* assembly [Aspose.Tasks](../../../)


