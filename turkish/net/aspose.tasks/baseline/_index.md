---
title: "Sınıf Baseline"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.Baseline sınıfı. Bir kaynağın temel değerlerini temsil eder"
type: docs
weight: 110
url: /tr/net/aspose.tasks/baseline/
---
## Baseline class

Bir kaynağın temel değerlerini temsil eder.

```csharp
public class Baseline : IComparable<Baseline>, IEquatable<Baseline>
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [Baseline](baseline/)() | Varsayılan yapıcı. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [BaselineNumber](../../aspose.tasks/baseline/baselinenumber/) { get; set; } | Bir temel veri kaydının benzersiz numarasını alır veya ayarlar. |
| [Bcwp](../../aspose.tasks/baseline/bcwp/) { get; set; } | Bir kaynağın bir proje için şu ana kadar gerçekleştirdiği işin bütçelenen maliyetini alır veya ayarlar. |
| [Bcws](../../aspose.tasks/baseline/bcws/) { get; set; } | Bir kaynak için planlanan işin bütçe maliyetini alır veya ayarlar. |
| [Cost](../../aspose.tasks/baseline/cost/) { get; set; } | Temel kaydedildiğinde bir kaynağın öngörülen maliyetini alır veya ayarlar. |
| [Work](../../aspose.tasks/baseline/work/) { get; set; } | Temel kaydedildiğinde bir kaynağa atanan işi alır veya ayarlar. Temel kaydedildiğinde bir kaynağa atanan iş miktarıdır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [CompareTo](../../aspose.tasks/baseline/compareto/)(Baseline) | IComparable arabirimi uygulaması. Bu örneği belirtilen Baseline nesnesiyle karşılaştırır. |
| [Equals](../../aspose.tasks/baseline/equals/#equals)(Baseline) | Bu örneğin belirtilen nesneye eşit olup olmadığını gösteren bir değer döndürür. |
| override [Equals](../../aspose.tasks/baseline/equals/#equals_1)(object) | Bu örneğin belirtilen nesneye eşit olup olmadığını gösteren bir değer döndürür. |
| override [GetHashCode](../../aspose.tasks/baseline/gethashcode/)() | Temel değer için bir karma kod (hash code) değeri döndürür. |
| [operator ==](../../aspose.tasks/baseline/op_equality/) | Bu örneğin belirtilen nesneye eşit olup olmadığını gösteren bir değer döndürür. |
| [operator &gt;](../../aspose.tasks/baseline/op_greaterthan/) | Bu örneğin belirtilen nesneden büyük olup olmadığını gösteren bir değer döndürür. |
| [operator &gt;=](../../aspose.tasks/baseline/op_greaterthanorequal/) | Bu örneğin belirtilen nesneden büyük veya ona eşit olup olmadığını gösteren bir değer döndürür. |
| [operator !=](../../aspose.tasks/baseline/op_inequality/) | Bu örneğin belirtilen nesneye eşit olmadığını gösteren bir değer döndürür. |
| [operator &lt;](../../aspose.tasks/baseline/op_lessthan/) | Bu örneğin belirtilen nesneden küçük olup olmadığını gösteren bir değer döndürür. |
| [operator &lt;=](../../aspose.tasks/baseline/op_lessthanorequal/) | Bu örneğin belirtilen nesneden küçük veya ona eşit olup olmadığını gösteren bir değer döndürür. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


