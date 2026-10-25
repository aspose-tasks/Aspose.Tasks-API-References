---
title: "Sınıf WBSCodeMaskCollection"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.WBSCodeMaskCollection sınıfı. WBSCodeMask nesnelerinin bir koleksiyonunu temsil eder"
type: docs
weight: 3510
url: /tr/net/aspose.tasks/wbscodemaskcollection/
---
## WBSCodeMaskCollection class

WBSCodeMask nesnelerinin bir koleksiyonunu temsil eder.

```csharp
public class WBSCodeMaskCollection : IList<WBSCodeMask>
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Count](../../aspose.tasks/wbscodemaskcollection/count/) { get; } | Bu koleksiyonda bulunan öğe sayısını alır. |
| [IsReadOnly](../../aspose.tasks/wbscodemaskcollection/isreadonly/) { get; } | Bu koleksiyonun yalnızca okunur olup olmadığını gösteren bir değer alır; aksi takdirde false. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [Add](../../aspose.tasks/wbscodemaskcollection/add/)(WBSCodeMask) | Belirtilen öğeyi bu koleksiyona ekler. |
| [Clear](../../aspose.tasks/wbscodemaskcollection/clear/)() | Bu koleksiyondaki tüm öğeleri kaldırır. |
| [Contains](../../aspose.tasks/wbscodemaskcollection/contains/)(WBSCodeMask) | Belirtilen öğe bu koleksiyonda bulunursa true, aksi takdirde false döndürür. |
| [CopyTo](../../aspose.tasks/wbscodemaskcollection/copyto/)(WBSCodeMask[], int) | Bu koleksiyonun öğelerini belirtilen diziye, belirtilen dizi indeksinden başlayarak kopyalar. |
| [GetEnumerator](../../aspose.tasks/wbscodemaskcollection/getenumerator/)() | Bu koleksiyon için bir enumerator döndürür. |
| [Remove](../../aspose.tasks/wbscodemaskcollection/remove/)(WBSCodeMask) | Bu koleksiyondan belirli bir nesnenin ilk oluşumunu kaldırır. |
| [ToList](../../aspose.tasks/wbscodemaskcollection/tolist/)() | Bir WBSCodeMaskCollection'ı [`WBSCodeMask`](../wbscodemask/) nesnelerinin listesine dönüştürür. |

## Örnekler

WBS kod maskesi koleksiyonu ile nasıl çalışılacağını gösterir.

```csharp
var project = new Project();

project.WBSCodeDefinition = new WBSCodeDefinition();
project.WBSCodeDefinition.GenerateWBSCode = true;
project.WBSCodeDefinition.VerifyUniqueness = true;
project.WBSCodeDefinition.CodePrefix = "CRS-";

project.WBSCodeDefinition.CodeMaskCollection.Clear();

var mask1 = new WBSCodeMask();
mask1.Length = 2;
mask1.Separator = "-";
mask1.Sequence = WBSSequence.OrderedNumbers;
project.WBSCodeDefinition.CodeMaskCollection.Add(mask1);

var mask2 = new WBSCodeMask();
mask2.Length = 1;
mask2.Separator = "-";
mask2.Sequence = WBSSequence.OrderedUppercaseLetters;
project.WBSCodeDefinition.CodeMaskCollection.Add(mask2);

Console.WriteLine("WBS Code mask's count: " + project.WBSCodeDefinition.CodeMaskCollection.Count);
Console.WriteLine("Is WBS Code mask collection read-only?: " + project.WBSCodeDefinition.CodeMaskCollection.IsReadOnly);
Console.WriteLine("Masks: ");
Console.WriteLine();
foreach (var wbsMask in project.WBSCodeDefinition.CodeMaskCollection)
{
    Console.WriteLine("Length: " + wbsMask.Length);
    Console.WriteLine("Level: " + wbsMask.Level);
    Console.WriteLine("Separator: " + wbsMask.Separator);
    Console.WriteLine("Sequence: " + wbsMask.Sequence);
    Console.WriteLine();
}

var task1 = project.RootTask.Children.Add("Task 1");
task1.Children.Add("Task 2");

project.Recalculate();

IEnumerable<Task> childTasks = project.RootTask.SelectAllChildTasks();
foreach (var childTask in childTasks)
{
    Console.WriteLine("Task name: " + childTask.Get(Tsk.Name));
    Console.WriteLine("Task WBS code: " + childTask.Get(Tsk.WBS));
}

project.WBSCodeDefinition.CodeMaskCollection.Remove(mask2);

if (project.WBSCodeDefinition.CodeMaskCollection.Contains(mask2))
{
    throw new InvalidOperationException("WBS code mask wasn't removed.");
}

var otherProject = new Project();
otherProject.WBSCodeDefinition = new WBSCodeDefinition();
otherProject.WBSCodeDefinition.GenerateWBSCode = true;
otherProject.WBSCodeDefinition.VerifyUniqueness = true;
otherProject.WBSCodeDefinition.CodePrefix = "CRS-";

// kod maskelerini diğer projeye kopyala
var masks = new WBSCodeMask[project.WBSCodeDefinition.CodeMaskCollection.Count];
project.WBSCodeDefinition.CodeMaskCollection.CopyTo(masks, 0);

foreach (var mask in masks)
{
    otherProject.WBSCodeDefinition.CodeMaskCollection.Add(mask);
}

List<WBSCodeMask> wbsMasks = otherProject.WBSCodeDefinition.CodeMaskCollection.ToList();
foreach (var wbsMask in wbsMasks)
{
    Console.WriteLine("Length: " + wbsMask.Length);
    Console.WriteLine("Level: " + wbsMask.Level);
    Console.WriteLine("Separator: " + wbsMask.Separator);
    Console.WriteLine("Sequence: " + wbsMask.Sequence);
    Console.WriteLine();
}

var otherTask1 = project.RootTask.Children.Add("Other task 1");
otherTask1.Children.Add("Other task 2");

otherProject.Recalculate();

Console.WriteLine("Print WBS codes of the other project: ");
IEnumerable<Task> otherChildTasks = otherProject.RootTask.SelectAllChildTasks();
foreach (var childTask in otherChildTasks)
{
    Console.WriteLine("Task name: " + childTask.Get(Tsk.Name));
    Console.WriteLine("Task WBS code: " + childTask.Get(Tsk.WBS));
}
```

### Ayrıca Bakınız

* class [WBSCodeMask](../wbscodemask/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


